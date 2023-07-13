# Comparing `tmp/PyBADS-1.0.0.tar.gz` & `tmp/PyBADS-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBADS-1.0.0.tar", last modified: Sat Jun 10 18:48:09 2023, max compression
+gzip compressed data, was "PyBADS-1.0.1.tar", last modified: Thu Jul 13 15:52:54 2023, max compression
```

## Comparing `PyBADS-1.0.0.tar` & `PyBADS-1.0.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.968071 PyBADS-1.0.0/
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.951071 PyBADS-1.0.0/.github/
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.955071 PyBADS-1.0.0/.github/workflows/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      504 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1297 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2223 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/merge-tests.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1054 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2258 2023-06-10 16:10:47.000000 PyBADS-1.0.0/.gitignore
--rw-r--r--   0 jeet      (1000) jeet      (1000)      619 2023-04-23 21:57:13.000000 PyBADS-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1517 2022-12-31 10:58:21.000000 PyBADS-1.0.0/LICENSE
--rw-r--r--   0 jeet      (1000) jeet      (1000)       12 2023-06-10 16:10:47.000000 PyBADS-1.0.0/MANIFEST.in
--rw-r--r--   0 jeet      (1000) jeet      (1000)    11820 2023-06-10 18:48:09.968071 PyBADS-1.0.0/PKG-INFO
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.956071 PyBADS-1.0.0/PyBADS.egg-info/
--rw-r--r--   0 jeet      (1000) jeet      (1000)    11820 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/PKG-INFO
--rw-r--r--   0 jeet      (1000) jeet      (1000)     3456 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/SOURCES.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)        1 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/dependency_links.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)      313 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/requires.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)        7 2023-06-10 18:48:09.000000 PyBADS-1.0.0/PyBADS.egg-info/top_level.txt
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9853 2023-06-10 18:40:03.000000 PyBADS-1.0.0/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)      137 2022-12-31 10:58:21.000000 PyBADS-1.0.0/environment.yml
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.956071 PyBADS-1.0.0/examples/
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10064 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_1_basic_usage.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9582 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_2_nonbox_constraints.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    14148 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_3_noisy_objective.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    17944 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_4_user_provided_noise.ipynb
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10359 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/pybads_example_5_extended_usage.ipynb
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.957071 PyBADS-1.0.0/examples/scripts/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      981 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_1_basic_usage.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1179 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_2_nonbox_constraints.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1307 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_3_noisy_objective.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1637 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_4_user_provided_noise.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1629 2023-06-10 16:10:47.000000 PyBADS-1.0.0/examples/scripts/pybads_example_5_extended_usage.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.957071 PyBADS-1.0.0/pybads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      556 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      635 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/__main__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      160 2023-06-10 18:48:09.000000 PyBADS-1.0.0/pybads/_version.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.957071 PyBADS-1.0.0/pybads/acquisition_functions/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       37 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/acquisition_functions/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1418 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/acquisition_functions/acq_fcn_lcb.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.958071 PyBADS-1.0.0/pybads/bads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      255 2023-06-10 07:26:33.000000 PyBADS-1.0.0/pybads/bads/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)      388 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)   103341 2023-06-10 18:40:03.000000 PyBADS-1.0.0/pybads/bads/bads.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2249 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/bads_dump.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    38330 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/gaussian_process_train.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5870 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/optimize_result.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.959071 PyBADS-1.0.0/pybads/bads/option_configs/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       53 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    15922 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/advanced_bads_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)      805 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/basic_bads_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/bads/option_configs/options_confs.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/option_configs/test_options.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)      108 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/bads/option_configs/test_options2.ini
--rw-r--r--   0 jeet      (1000) jeet      (1000)     7371 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/bads/options.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.959071 PyBADS-1.0.0/pybads/decorators/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      573 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/decorators/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)       51 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/decorators/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2175 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/decorators/handle_0D_1D_input.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1779 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/function_examples.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.960071 PyBADS-1.0.0/pybads/function_logger/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      106 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/function_logger/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1731 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/function_logger/constraints_check.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    16376 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/function_logger/function_logger.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.960071 PyBADS-1.0.0/pybads/init_functions/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       35 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/init_functions/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1256 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/init_functions/init_sobol.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.960071 PyBADS-1.0.0/pybads/poll/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/poll/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1403 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/poll/poll_mads_2n.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.961071 PyBADS-1.0.0/pybads/search/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      177 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/search/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10559 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/search/es_search.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1659 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/search/grid_functions.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5383 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/search/search_hedge.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.962071 PyBADS-1.0.0/pybads/stats/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      110 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/stats/README.md
--rw-r--r--   0 jeet      (1000) jeet      (1000)       87 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/stats/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1197 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/stats/get_hpd.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     8723 2023-06-10 07:27:45.000000 PyBADS-1.0.0/pybads/stats/kde1d.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1435 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/stats/kldiv_mvn.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.962071 PyBADS-1.0.0/pybads/testing/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/__init__.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.964071 PyBADS-1.0.0/pybads/testing/bads/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      349 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/X.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      202 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/dF.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)      211 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/dF_gplogjoint.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1286 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/hyp.dat
--rw-r--r--   0 jeet      (1000) jeet      (1000)       89 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/mu.dat
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.964071 PyBADS-1.0.0/pybads/testing/bads/poll/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/poll/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      551 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/poll/test_poll_mads.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.965071 PyBADS-1.0.0/pybads/testing/bads/scripts/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      747 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/ackley_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     2629 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1874 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/bads_rosenbrock_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      908 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/non_bound_example.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      780 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/scripts/rastrigin_example.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.965071 PyBADS-1.0.0/pybads/testing/bads/search/
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5578 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/search/test_search.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     3482 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_bads_optimization.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     6697 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_gaussian_process_train.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      132 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_init_conf.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4933 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/test_iteration_history.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      192 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/bads/y.dat
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.966071 PyBADS-1.0.0/pybads/testing/decorators/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/decorators/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4746 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.966071 PyBADS-1.0.0/pybads/testing/function_logger/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/function_logger/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     9336 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/function_logger/test_function_logger.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      240 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/run_tests.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.967071 PyBADS-1.0.0/pybads/testing/variable_transformer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/variable_transformer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     5524 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pybads/testing/variable_transformer/test_variable_transformer.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.967071 PyBADS-1.0.0/pybads/utils/
--rw-r--r--   0 jeet      (1000) jeet      (1000)      119 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     4359 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/iteration_history.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)      117 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/period_check.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.967071 PyBADS-1.0.0/pybads/utils/timer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-1.0.0/pybads/utils/timer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1544 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/utils/timer/timer.py
-drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-06-10 18:48:09.968071 PyBADS-1.0.0/pybads/variable_transformer/
--rw-r--r--   0 jeet      (1000) jeet      (1000)       55 2023-04-23 21:57:13.000000 PyBADS-1.0.0/pybads/variable_transformer/__init__.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)    10171 2023-06-10 18:40:03.000000 PyBADS-1.0.0/pybads/variable_transformer/variables_transformer.py
--rw-r--r--   0 jeet      (1000) jeet      (1000)     1477 2023-06-10 16:10:47.000000 PyBADS-1.0.0/pyproject.toml
--rw-r--r--   0 jeet      (1000) jeet      (1000)       38 2023-06-10 18:48:09.968071 PyBADS-1.0.0/setup.cfg
--rw-r--r--   0 jeet      (1000) jeet      (1000)      169 2023-04-23 21:57:13.000000 PyBADS-1.0.0/setup.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.097682 PyBADS-1.0.1/.github/
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.100682 PyBADS-1.0.1/.github/workflows/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      504 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1297 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2223 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/merge-tests.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1054 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2258 2023-06-10 16:10:47.000000 PyBADS-1.0.1/.gitignore
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      619 2023-04-23 21:57:13.000000 PyBADS-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1517 2022-12-31 10:58:21.000000 PyBADS-1.0.1/LICENSE
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       12 2023-06-10 16:10:47.000000 PyBADS-1.0.1/MANIFEST.in
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    12476 2023-07-13 15:52:54.112682 PyBADS-1.0.1/PKG-INFO
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.100682 PyBADS-1.0.1/PyBADS.egg-info/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    12476 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/PKG-INFO
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     3456 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/SOURCES.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        1 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/dependency_links.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      313 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/requires.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        7 2023-07-13 15:52:54.000000 PyBADS-1.0.1/PyBADS.egg-info/top_level.txt
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10509 2023-07-07 08:40:58.000000 PyBADS-1.0.1/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      137 2022-12-31 10:58:21.000000 PyBADS-1.0.1/environment.yml
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.101682 PyBADS-1.0.1/examples/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10228 2023-07-07 08:40:58.000000 PyBADS-1.0.1/examples/pybads_example_1_basic_usage.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9736 2023-07-07 08:40:58.000000 PyBADS-1.0.1/examples/pybads_example_2_nonbox_constraints.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    14356 2023-07-07 08:40:58.000000 PyBADS-1.0.1/examples/pybads_example_3_noisy_objective.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    17944 2023-07-07 08:30:17.000000 PyBADS-1.0.1/examples/pybads_example_4_user_provided_noise.ipynb
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10359 2023-07-07 08:30:17.000000 PyBADS-1.0.1/examples/pybads_example_5_extended_usage.ipynb
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.102682 PyBADS-1.0.1/examples/scripts/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      981 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_1_basic_usage.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1179 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_2_nonbox_constraints.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1307 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_3_noisy_objective.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1637 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_4_user_provided_noise.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1629 2023-06-10 16:10:47.000000 PyBADS-1.0.1/examples/scripts/pybads_example_5_extended_usage.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.103682 PyBADS-1.0.1/pybads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      556 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      635 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/__main__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      160 2023-07-13 15:52:53.000000 PyBADS-1.0.1/pybads/_version.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.103682 PyBADS-1.0.1/pybads/acquisition_functions/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       37 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/acquisition_functions/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1418 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/acquisition_functions/acq_fcn_lcb.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.104682 PyBADS-1.0.1/pybads/bads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      255 2023-06-10 07:26:33.000000 PyBADS-1.0.1/pybads/bads/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      388 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)   103341 2023-06-10 18:40:03.000000 PyBADS-1.0.1/pybads/bads/bads.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2249 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/bads_dump.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    38330 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/gaussian_process_train.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5870 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/optimize_result.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.105682 PyBADS-1.0.1/pybads/bads/option_configs/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       53 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    15922 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/advanced_bads_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      805 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/basic_bads_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/bads/option_configs/options_confs.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       99 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/option_configs/test_options.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      108 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/bads/option_configs/test_options2.ini
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     7371 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/bads/options.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.105682 PyBADS-1.0.1/pybads/decorators/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      573 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/decorators/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       51 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/decorators/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2175 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/decorators/handle_0D_1D_input.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1779 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/function_examples.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.106682 PyBADS-1.0.1/pybads/function_logger/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      106 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/function_logger/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1731 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/function_logger/constraints_check.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    16376 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/function_logger/function_logger.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.106682 PyBADS-1.0.1/pybads/init_functions/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       35 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/init_functions/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1256 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/init_functions/init_sobol.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.106682 PyBADS-1.0.1/pybads/poll/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/poll/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1403 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/poll/poll_mads_2n.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.107682 PyBADS-1.0.1/pybads/search/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      177 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/search/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10448 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/search/es_search.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1659 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/search/grid_functions.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5383 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/search/search_hedge.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.107682 PyBADS-1.0.1/pybads/stats/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      110 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/stats/README.md
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       87 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/stats/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1197 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/stats/get_hpd.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     8723 2023-06-10 07:27:45.000000 PyBADS-1.0.1/pybads/stats/kde1d.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1435 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/stats/kldiv_mvn.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.108682 PyBADS-1.0.1/pybads/testing/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/__init__.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.109682 PyBADS-1.0.1/pybads/testing/bads/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      349 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/X.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      202 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/dF.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      211 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/dF_gplogjoint.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1286 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/hyp.dat
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       89 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/mu.dat
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.109682 PyBADS-1.0.1/pybads/testing/bads/poll/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/poll/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      551 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/poll/test_poll_mads.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.110682 PyBADS-1.0.1/pybads/testing/bads/scripts/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      747 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/ackley_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     2631 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1874 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/bads_rosenbrock_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      908 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/non_bound_example.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      780 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/scripts/rastrigin_example.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.110682 PyBADS-1.0.1/pybads/testing/bads/search/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5583 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/testing/bads/search/test_search.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     3953 2023-07-07 08:40:58.000000 PyBADS-1.0.1/pybads/testing/bads/test_bads_optimization.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     6697 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/test_gaussian_process_train.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      132 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/test_init_conf.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4933 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/test_iteration_history.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      192 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/bads/y.dat
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.110682 PyBADS-1.0.1/pybads/testing/decorators/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/decorators/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4746 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.111682 PyBADS-1.0.1/pybads/testing/function_logger/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/function_logger/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     9336 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/function_logger/test_function_logger.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      240 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/run_tests.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.111682 PyBADS-1.0.1/pybads/testing/variable_transformer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)        0 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/variable_transformer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     5524 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pybads/testing/variable_transformer/test_variable_transformer.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/pybads/utils/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      119 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     4359 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/iteration_history.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      117 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/period_check.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/pybads/utils/timer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       39 2022-12-31 10:58:21.000000 PyBADS-1.0.1/pybads/utils/timer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1544 2023-04-23 21:57:13.000000 PyBADS-1.0.1/pybads/utils/timer/timer.py
+drwxr-xr-x   0 jeet      (1000) jeet      (1000)        0 2023-07-13 15:52:54.112682 PyBADS-1.0.1/pybads/variable_transformer/
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       55 2023-06-27 15:19:01.000000 PyBADS-1.0.1/pybads/variable_transformer/__init__.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)    10171 2023-06-10 18:40:03.000000 PyBADS-1.0.1/pybads/variable_transformer/variables_transformer.py
+-rw-r--r--   0 jeet      (1000) jeet      (1000)     1477 2023-06-10 16:10:47.000000 PyBADS-1.0.1/pyproject.toml
+-rw-r--r--   0 jeet      (1000) jeet      (1000)       38 2023-07-13 15:52:54.113682 PyBADS-1.0.1/setup.cfg
+-rw-r--r--   0 jeet      (1000) jeet      (1000)      169 2023-04-23 21:57:13.000000 PyBADS-1.0.1/setup.py
```

### Comparing `PyBADS-1.0.0/.github/workflows/docs.yml` & `PyBADS-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/.github/workflows/merge-tests.yml` & `PyBADS-1.0.1/.github/workflows/merge-tests.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/.github/workflows/tests.yml` & `PyBADS-1.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/.gitignore` & `PyBADS-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/.pre-commit-config.yaml` & `PyBADS-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/LICENSE` & `PyBADS-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/PKG-INFO` & `PyBADS-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBADS
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bayesian Adaptive Direct Search in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2022, acerbilab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -150,32 +150,45 @@
 
 If you have trouble doing something with PyBADS, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyBADS, your problems & applications;
 - [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub.
 
 ## References and citation
 
-1. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
+1. Singh, S. G. & Acerbi, L. (2023). PyBADS: Fast and robust black-box optimization in Python. *arXiv preprint*. https://arxiv.org/abs/2306.15576
 
-You can cite PyBADS in your work with something along the lines of
+2. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
 
-> We optimized the log likelihoods of our models using Bayesian adaptive direct search (BADS; Acerbi and Ma, 2017). BADS alternates between a series of fast, local Bayesian optimization steps and a systematic, slower exploration of a mesh grid.
+
+Please cite both references if you use PyBADS in your work (the 2017 paper introduced the framework, and the latest one is its Python library). You can cite PyBADS in your work with something along the lines of
+
+> We optimized the log likelihoods of our models using Bayesian adaptive direct search (BADS; Acerbi and Ma, 2017), via the PyBADS software (Singh and Acerbi, 2023). PyBADS alternates between a series of fast, local Bayesian optimization steps and a systematic, slower exploration of a mesh grid.
 
 Besides formal citations, you can demonstrate your appreciation for PyBADS in the following ways:
 
-- *Star :star:* the BADS repository on GitHub;
+- *Star :star:* the PyBADS repository on GitHub;
 - [Subscribe](http://eepurl.com/idcvc9) to the lab's newsletter for news and updates (new features, bug fixes, new releases, etc.);
 - [Follow Luigi Acerbi on Twitter](https://twitter.com/AcerbiLuigi) for updates about BADS/PyBADS and other projects;
 - Tell us about your model-fitting problem and your experience with PyBADS (positive or negative) in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions).
 
 *Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python ([PyVBMC](https://github.com/acerbilab/pyvbmc)), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.
 
 ### BibTeX
 
 ```BibTeX
+@article{singh2023pybads,
+  title={{PyBADS}: {F}ast and robust black-box optimization in {P}ython}, 
+  author={Gurjeet Sangra Singh and Luigi Acerbi},
+  publisher = {preprint},
+  journal = {{arXiv}},
+  url = {https://arxiv.org/abs/2306.15576},
+  doi = {10.48550/ARXIV.2306.15576},
+  year = {2023},
+}
+
 @article{acerbi2017practical,
     title={Practical {B}ayesian Optimization for Model Fitting with {B}ayesian Adaptive Direct Search},
     author={Acerbi, Luigi and Ma, Wei Ji},
     journal={Advances in Neural Information Processing Systems},
     volume={30},
     pages={1834--1844},
     year={2017}
@@ -184,8 +197,8 @@
 
 ### License
 
 PyBADS is released under the terms of the [BSD 3-Clause License](LICENSE).
 
 ### Acknowledgments
 
-PyBADS was developed by [members](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/people) (past and current) of the [Machine and Human Intelligence Lab](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/) at the University of Helsinki. Work on the PyBADS package was supported by the Academy of Finland Flagship programme: [Finnish Center for Artificial Intelligence FCAI](https://fcai.fi/).
+PyBADS was developed by [members](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/people) (past and current) of the [Machine and Human Intelligence Lab](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/) at the University of Helsinki. Work on the PyBADS package was supported by the Research Council of Finland Flagship programme: [Finnish Center for Artificial Intelligence FCAI](https://fcai.fi/).
```

### Comparing `PyBADS-1.0.0/PyBADS.egg-info/PKG-INFO` & `PyBADS-1.0.1/PyBADS.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBADS
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bayesian Adaptive Direct Search in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2022, acerbilab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -150,32 +150,45 @@
 
 If you have trouble doing something with PyBADS, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyBADS, your problems & applications;
 - [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub.
 
 ## References and citation
 
-1. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
+1. Singh, S. G. & Acerbi, L. (2023). PyBADS: Fast and robust black-box optimization in Python. *arXiv preprint*. https://arxiv.org/abs/2306.15576
 
-You can cite PyBADS in your work with something along the lines of
+2. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
 
-> We optimized the log likelihoods of our models using Bayesian adaptive direct search (BADS; Acerbi and Ma, 2017). BADS alternates between a series of fast, local Bayesian optimization steps and a systematic, slower exploration of a mesh grid.
+
+Please cite both references if you use PyBADS in your work (the 2017 paper introduced the framework, and the latest one is its Python library). You can cite PyBADS in your work with something along the lines of
+
+> We optimized the log likelihoods of our models using Bayesian adaptive direct search (BADS; Acerbi and Ma, 2017), via the PyBADS software (Singh and Acerbi, 2023). PyBADS alternates between a series of fast, local Bayesian optimization steps and a systematic, slower exploration of a mesh grid.
 
 Besides formal citations, you can demonstrate your appreciation for PyBADS in the following ways:
 
-- *Star :star:* the BADS repository on GitHub;
+- *Star :star:* the PyBADS repository on GitHub;
 - [Subscribe](http://eepurl.com/idcvc9) to the lab's newsletter for news and updates (new features, bug fixes, new releases, etc.);
 - [Follow Luigi Acerbi on Twitter](https://twitter.com/AcerbiLuigi) for updates about BADS/PyBADS and other projects;
 - Tell us about your model-fitting problem and your experience with PyBADS (positive or negative) in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions).
 
 *Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python ([PyVBMC](https://github.com/acerbilab/pyvbmc)), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.
 
 ### BibTeX
 
 ```BibTeX
+@article{singh2023pybads,
+  title={{PyBADS}: {F}ast and robust black-box optimization in {P}ython}, 
+  author={Gurjeet Sangra Singh and Luigi Acerbi},
+  publisher = {preprint},
+  journal = {{arXiv}},
+  url = {https://arxiv.org/abs/2306.15576},
+  doi = {10.48550/ARXIV.2306.15576},
+  year = {2023},
+}
+
 @article{acerbi2017practical,
     title={Practical {B}ayesian Optimization for Model Fitting with {B}ayesian Adaptive Direct Search},
     author={Acerbi, Luigi and Ma, Wei Ji},
     journal={Advances in Neural Information Processing Systems},
     volume={30},
     pages={1834--1844},
     year={2017}
@@ -184,8 +197,8 @@
 
 ### License
 
 PyBADS is released under the terms of the [BSD 3-Clause License](LICENSE).
 
 ### Acknowledgments
 
-PyBADS was developed by [members](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/people) (past and current) of the [Machine and Human Intelligence Lab](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/) at the University of Helsinki. Work on the PyBADS package was supported by the Academy of Finland Flagship programme: [Finnish Center for Artificial Intelligence FCAI](https://fcai.fi/).
+PyBADS was developed by [members](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/people) (past and current) of the [Machine and Human Intelligence Lab](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/) at the University of Helsinki. Work on the PyBADS package was supported by the Research Council of Finland Flagship programme: [Finnish Center for Artificial Intelligence FCAI](https://fcai.fi/).
```

### Comparing `PyBADS-1.0.0/PyBADS.egg-info/SOURCES.txt` & `PyBADS-1.0.1/PyBADS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/README.md` & `PyBADS-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -111,32 +111,45 @@
 
 If you have trouble doing something with PyBADS, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyBADS, your problems & applications;
 - [Open an issue](https://github.com/acerbilab/pybads/issues/new) on GitHub.
 
 ## References and citation
 
-1. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
+1. Singh, S. G. & Acerbi, L. (2023). PyBADS: Fast and robust black-box optimization in Python. *arXiv preprint*. https://arxiv.org/abs/2306.15576
 
-You can cite PyBADS in your work with something along the lines of
+2. Acerbi, L. & Ma, W. J. (2017). Practical Bayesian Optimization for Model Fitting with Bayesian Adaptive Direct Search. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1705.04405), [NeurIPS Proceedings](https://papers.nips.cc/paper/2017/hash/df0aab058ce179e4f7ab135ed4e641a9-Abstract.html))
 
-> We optimized the log likelihoods of our models using Bayesian adaptive direct search (BADS; Acerbi and Ma, 2017). BADS alternates between a series of fast, local Bayesian optimization steps and a systematic, slower exploration of a mesh grid.
+
+Please cite both references if you use PyBADS in your work (the 2017 paper introduced the framework, and the latest one is its Python library). You can cite PyBADS in your work with something along the lines of
+
+> We optimized the log likelihoods of our models using Bayesian adaptive direct search (BADS; Acerbi and Ma, 2017), via the PyBADS software (Singh and Acerbi, 2023). PyBADS alternates between a series of fast, local Bayesian optimization steps and a systematic, slower exploration of a mesh grid.
 
 Besides formal citations, you can demonstrate your appreciation for PyBADS in the following ways:
 
-- *Star :star:* the BADS repository on GitHub;
+- *Star :star:* the PyBADS repository on GitHub;
 - [Subscribe](http://eepurl.com/idcvc9) to the lab's newsletter for news and updates (new features, bug fixes, new releases, etc.);
 - [Follow Luigi Acerbi on Twitter](https://twitter.com/AcerbiLuigi) for updates about BADS/PyBADS and other projects;
 - Tell us about your model-fitting problem and your experience with PyBADS (positive or negative) in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions).
 
 *Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out Variational Bayesian Monte Carlo for Python ([PyVBMC](https://github.com/acerbilab/pyvbmc)), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.
 
 ### BibTeX
 
 ```BibTeX
+@article{singh2023pybads,
+  title={{PyBADS}: {F}ast and robust black-box optimization in {P}ython}, 
+  author={Gurjeet Sangra Singh and Luigi Acerbi},
+  publisher = {preprint},
+  journal = {{arXiv}},
+  url = {https://arxiv.org/abs/2306.15576},
+  doi = {10.48550/ARXIV.2306.15576},
+  year = {2023},
+}
+
 @article{acerbi2017practical,
     title={Practical {B}ayesian Optimization for Model Fitting with {B}ayesian Adaptive Direct Search},
     author={Acerbi, Luigi and Ma, Wei Ji},
     journal={Advances in Neural Information Processing Systems},
     volume={30},
     pages={1834--1844},
     year={2017}
@@ -145,8 +158,8 @@
 
 ### License
 
 PyBADS is released under the terms of the [BSD 3-Clause License](LICENSE).
 
 ### Acknowledgments
 
-PyBADS was developed by [members](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/people) (past and current) of the [Machine and Human Intelligence Lab](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/) at the University of Helsinki. Work on the PyBADS package was supported by the Academy of Finland Flagship programme: [Finnish Center for Artificial Intelligence FCAI](https://fcai.fi/).
+PyBADS was developed by [members](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/people) (past and current) of the [Machine and Human Intelligence Lab](https://www.helsinki.fi/en/researchgroups/machine-and-human-intelligence/) at the University of Helsinki. Work on the PyBADS package was supported by the Research Council of Finland Flagship programme: [Finnish Center for Artificial Intelligence FCAI](https://fcai.fi/).
```

### Comparing `PyBADS-1.0.0/examples/pybads_example_1_basic_usage.ipynb` & `PyBADS-1.0.1/examples/pybads_example_1_basic_usage.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9840435606060607%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 3: {'source': "*

 * *            "{insert: [(19, '\\n')]}, 'attachments': OrderedDict()}, 4: {'attachments': "*

 * *            "OrderedDict()}, 6: {'attachments': OrderedDict()}, 8: {'attachments': OrderedDict()}, "*

 * *            "10: {'attachments': OrderedDict()}}"}*

```diff
@@ -1,18 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "eeb3e178",
             "metadata": {},
             "source": [
                 "# PyBADS Example 1: Basic usage"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "7f191949",
             "metadata": {},
             "source": [
                 "In this introductory example, we will show a simple usage of Bayesian Adaptive Direct Search (BADS) to perform optimization of a synthetic target function.\n",
                 "\n",
                 "This notebook is Part 1 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
@@ -27,14 +29,15 @@
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from pybads.bads import BADS"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "f6e7fc85",
             "metadata": {},
             "source": [
                 "## 0. What is (Py)BADS?\n",
                 "\n",
                 "BADS is a fast hybrid Bayesian optimization algorithm designed to solve difficult optimization problems, in particular related to parameter estimation -- aka model fitting -- of computational models (e.g., via maximum-likelihood or maximum-a-posteriori estimation). **PyBADS is its Python implementation**.\n",
@@ -50,21 +53,23 @@
                 "BADS requires no specific tuning and runs off-the-shelf like other built-in Python optimizers (e.g., from `scipy.optimize.minimize`).\n",
                 "\n",
                 "*Note*: If you are interested in estimating posterior distributions (i.e., uncertainty and error bars) over model parameters, and not just point estimates, you might also want to check out [Variational Bayesian Monte Carlo for Python (PyVBMC)](https://github.com/acerbilab/pyvbmc), a package for Bayesian posterior and model inference which can be used in synergy with PyBADS.\n",
                 "\n",
                 "### Optimization problem\n",
                 "\n",
                 "Formally, the goal of BADS is to *minimize* a target (or objective) function $f(\\mathbf{x}): \\mathbb{R}^D \\rightarrow \\mathbb{R}$, for $\\mathbf{x} \\in \\mathbb{R}^D$,\n",
+                "\n",
                 "$$\n",
                 "\\mathbf{x}^\\star = \\arg\\min_\\mathbf{x} f(\\mathbf{x}) \\qquad \\text{with} \\; \\text{lower_bounds}_d \\le x_d \\le \\text{upper_bounds}_d \\; \\text{ for } 1\\le d \\le D,\n",
                 "$$\n",
                 "where $D$ is the dimensionality of the problem and `lower_bounds`, `upper_bounds` are arrays representing lower/upper bound constraints, which can be set to infinite for unbounded parameters."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "2456c17e",
             "metadata": {},
             "source": [
                 "## 1. Problem setup\n",
                 "\n",
                 "Here we show PyBADS at work on [Rosenbrock's banana function](https://en.wikipedia.org/wiki/Rosenbrock_function) in 2D as target function.  \n",
@@ -94,14 +99,15 @@
                 "upper_bounds = np.array([20, 20])\n",
                 "plausible_lower_bounds = np.array([-5, -5])\n",
                 "plausible_upper_bounds = np.array([5, 5])\n",
                 "x0 = np.array([0, 0]);        # Starting point"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "d6fb12aa",
             "metadata": {},
             "source": [
                 "## 2. Initialize and run the optimization\n",
                 "\n",
                 "Then, we initialize a `bads` instance which takes care of the optimization. For now, we use default options.  \n",
@@ -143,14 +149,15 @@
             ],
             "source": [
                 "bads = BADS(target, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds)\n",
                 "optimize_result = bads.optimize()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "2cc75241",
             "metadata": {},
             "source": [
                 "## 3. Results and conclusions\n",
                 "\n",
                 "We examine now the result of the optimization stored in `optimize_result`. The most important keys are the location of the minimum, `optimize_result['x']`, and the value of the function at the minimum, `optimize_result['fval']`."
@@ -176,14 +183,15 @@
                 "fval = optimize_result['fval']\n",
                 "\n",
                 "print(f\"BADS minimum at: x_min = {x_min.flatten()}, fval = {fval:.4g}\")\n",
                 "print(f\"total f-count: {optimize_result['func_count']}, time: {round(optimize_result['total_time'], 2)} s\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "d7d79d83",
             "metadata": {},
             "source": [
                 "For reference, the true minimum of the Rosenbrock function is at $\\textbf{x}^\\star = [1, 1]$, where $f^\\star = 0$.  \n",
                 "\n",
                 "In conclusion, PyBADS found the solution with a fairly small number of function evaluations (`f-count`), which is particularly important if the target function is mildly-to-very expensive to compute as in many computational models.\n",
```

### Comparing `PyBADS-1.0.0/examples/pybads_example_2_nonbox_constraints.ipynb` & `PyBADS-1.0.1/examples/pybads_example_2_nonbox_constraints.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9840909090909091%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 3: "*

 * *            "{'attachments': OrderedDict()}, 4: {'attachments': OrderedDict()}, 6: {'attachments': "*

 * *            "OrderedDict()}, 8: {'attachments': OrderedDict()}, 10: {'attachments': "*

 * *            'OrderedDict()}}'}*

```diff
@@ -1,18 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "e48db32f",
             "metadata": {},
             "source": [
                 "# PyBADS Example 2: Non-box constraints"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "810b5d8b",
             "metadata": {},
             "source": [
                 "In this example, we will show how to set more complex constraints in PyBADS, besides a simple bounded box.\n",
                 "\n",
                 "This notebook is Part 2 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
@@ -27,14 +29,15 @@
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from pybads import BADS"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "ed499dff",
             "metadata": {},
             "source": [
                 "## 0. Constrained optimization\n",
                 "\n",
                 "PyBADS naturally supports box constraints `lb` and `ub`, as we saw in the [previous example](./pybads_example_1_basic_usage.ipynb). However, some optimization problems might have more complex constraints over the variables. Formally, we may wish to solve the problem\n",
@@ -44,14 +47,15 @@
                 "$$\n",
                 "where $\\mathcal{X} \\subseteq \\mathbb{R}^D$ is the admissible region for the optimization.\n",
                 "\n",
                 "We can do this in PyBADS by providing a function `non_box_cons` that defines constraints *violation*, that is a function $g(\\mathbf{x})$ which returns `True` if $\\mathbf{x} \\notin \\mathcal{X}$ (and `False` otherwise), as demonstrated below."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "fccd1931",
             "metadata": {},
             "source": [
                 "## 1. Problem setup\n",
                 "\n",
                 "We optimize [Rosenbrock's banana function](https://en.wikipedia.org/wiki/Rosenbrock_function) in 2D as in the [previous example](./pybads_example_1_basic_usage.ipynb), but here we force the input to stay within a circle with unit radius.\n",
@@ -85,14 +89,15 @@
                 "    \"\"\"Return constraints violation outside the unit circle.\"\"\"\n",
                 "    x_2d = np.atleast_2d(x)\n",
                 "    # Note that nonboxcons assumes the function takes a 2D input \n",
                 "    return np.sum(x_2d**2, axis=1) > 1."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "363e280e",
             "metadata": {},
             "source": [
                 "## 2. Run the optimization\n",
                 "\n",
                 "We initialize `bads` with the non-box constraints defined by `non_box_cons`. Note that we also still specify standard box constraints `lower_bounds` and `upper_bounds`, as this will help the search.\n",
@@ -146,14 +151,15 @@
             ],
             "source": [
                 "bads = BADS(rosenbrocks_fcn, x0, lower_bounds, upper_bounds, non_box_cons=circle_constr)\n",
                 "optimize_result = bads.optimize()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "4a7af7d8",
             "metadata": {},
             "source": [
                 "## 3. Results and conclusions"
             ]
         },
@@ -179,14 +185,15 @@
                 "\n",
                 "print(f\"BADS minimum at: x_min = {x_min.flatten()}, fval = {fval:.4g}\")\n",
                 "print(f\"total f-count: {optimize_result['func_count']}, time: {round(optimize_result['total_time'], 2)} s\")\n",
                 "print(f\"Problem type: {optimize_result['problem_type']}\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "d3ace561",
             "metadata": {},
             "source": [
                 "The true global minimum of the Rosenbrock function under these constraints is at $\\textbf{x}^\\star = [0.786,0.618]$, where $f^\\star = 0.0457$.\n",
                 "\n",
                 "### Remarks\n",
```

### Comparing `PyBADS-1.0.0/examples/pybads_example_3_noisy_objective.ipynb` & `PyBADS-1.0.1/examples/pybads_example_3_noisy_objective.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.983829365079365%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 3: {'source': "*

 * *            "{insert: [(5, '\\n')]}, 'attachments': OrderedDict()}, 4: {'attachments': "*

 * *            "OrderedDict()}, 6: {'attachments': OrderedDict()}, 8: {'attachments': OrderedDict()}, "*

 * *            "10: {'attachments': OrderedDict()}, 12: {'attachments': OrderedDict()}, 13: "*

 * *            "{'attachments': OrderedDict()}}"}*

```diff
@@ -1,18 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "e48db32f",
             "metadata": {},
             "source": [
                 "# PyBADS Example 3: Noisy objective function"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "810b5d8b",
             "metadata": {},
             "source": [
                 "In this example, we will show how to run PyBADS on a noisy target.\n",
                 "\n",
                 "This notebook is Part 3 of a series of notebooks in which we present various example usages for BADS with the PyBADS package.\n",
@@ -27,29 +29,32 @@
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from pybads import BADS"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "18652cfa",
             "metadata": {},
             "source": [
                 "## 0. Noisy optimization\n",
                 "\n",
                 "PyBADS is also able to optimize *noisy* objective functions. A noisy (or stochastic) objective function is an objective that will return different results if evaluated twice at the same point $\\mathbf{x}$. Conversely, a non-noisy objective function is known as noiseless or deterministic. For example, noisy objectives are common in model fitting when the model is evaluated through simulation (e.g., via sampling aka Monte Carlo methods).\n",
                 "\n",
                 "For a noisy objective, PyBADS aims to minimize the *expected value* of $f(\\mathbf{x})$:\n",
+                "\n",
                 "$$\n",
                 "\\mathbf{x}^\\star = \\arg\\min_{\\mathbf{x} \\in \\mathcal{X} \\subseteq \\mathbb{R}^D} \\mathbb{E}\\left[f(\\mathbf{x})\\right].\n",
                 "$$"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "fccd1931",
             "metadata": {},
             "source": [
                 "## 1. Problem setup\n",
                 "\n",
                 "For this example, we take as target a quadratic function and we add i.i.d. Gaussian noise to it (*noisy sphere*). In a real case, the noise would arise from some stochastic process in the calculation of the target.\n",
@@ -85,14 +90,15 @@
                 "    \"uncertainty_handling\": True,\n",
                 "    \"max_fun_evals\": 300,\n",
                 "    \"noise_final_samples\": 100\n",
                 "}"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "363e280e",
             "metadata": {},
             "source": [
                 "## 2. Run the optimization\n",
                 "\n",
                 "We run `bads` with the user-defined `options`."
@@ -160,14 +166,15 @@
                 "bads = BADS(\n",
                 "    noisy_sphere, x0, lower_bounds, upper_bounds, plausible_lower_bounds, plausible_upper_bounds, options=options\n",
                 ")\n",
                 "optimize_result = bads.optimize()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "4a7af7d8",
             "metadata": {},
             "source": [
                 "## 3. Results and conclusions\n",
                 "\n",
                 "First, note that in this case `optimize_result['fval']` is the *estimated* function value at `optimize_result['x']`, obtained by taking the mean of `options['noise_final_samples']` target evaluations (`noise_final_samples = 10` by default, but here we used 100). The uncertainty of the value of the function at the returned solution, `optimize_result['fsd']`, is the [standard error](https://en.wikipedia.org/wiki/Standard_error) of the mean.\n",
@@ -198,14 +205,15 @@
                 "\n",
                 "print(f\"BADS minimum at: x_min = {x_min.flatten()}, fval (estimated) = {fval:.4g} +/- {fsd:.2g}\")\n",
                 "print(f\"total f-count: {optimize_result['func_count']}, time: {round(optimize_result['total_time'], 2)} s\")\n",
                 "print(f\"final evaluations (shape): {optimize_result['yval_vec'].shape}\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "499c04d1",
             "metadata": {},
             "source": [
                 "We can also check the ground-truth value of the target function at the returned point once we remove the noise:"
             ]
         },
@@ -224,22 +232,24 @@
                 }
             ],
             "source": [
                 "print(f\"The true, noiseless value of f(x_min) is {noisy_sphere(x_min,sigma=0)[0]:.3g}.\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "d3ace561",
             "metadata": {},
             "source": [
                 "Compare this to the true global minimum of the sphere function at $\\textbf{x}^\\star = [0,0]$, where $f^\\star = 0$."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "dfcef7ec",
             "metadata": {},
             "source": [
                 "### Remarks\n",
                 "    \n",
                 "- While PyBADS can handle noisy targets, it cannot handle arbitrarily large noise.\n",
```

### Comparing `PyBADS-1.0.0/examples/pybads_example_4_user_provided_noise.ipynb` & `PyBADS-1.0.1/examples/pybads_example_4_user_provided_noise.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/examples/pybads_example_5_extended_usage.ipynb` & `PyBADS-1.0.1/examples/pybads_example_5_extended_usage.ipynb`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/examples/scripts/pybads_example_1_basic_usage.py` & `PyBADS-1.0.1/examples/scripts/pybads_example_1_basic_usage.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/examples/scripts/pybads_example_2_nonbox_constraints.py` & `PyBADS-1.0.1/examples/scripts/pybads_example_2_nonbox_constraints.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/examples/scripts/pybads_example_3_noisy_objective.py` & `PyBADS-1.0.1/examples/scripts/pybads_example_3_noisy_objective.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/examples/scripts/pybads_example_4_user_provided_noise.py` & `PyBADS-1.0.1/examples/scripts/pybads_example_4_user_provided_noise.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/examples/scripts/pybads_example_5_extended_usage.py` & `PyBADS-1.0.1/examples/scripts/pybads_example_5_extended_usage.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/__init__.py` & `PyBADS-1.0.1/pybads/__init__.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/__main__.py` & `PyBADS-1.0.1/pybads/__main__.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/acquisition_functions/acq_fcn_lcb.py` & `PyBADS-1.0.1/pybads/acquisition_functions/acq_fcn_lcb.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/bads.py` & `PyBADS-1.0.1/pybads/bads/bads.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/bads_dump.py` & `PyBADS-1.0.1/pybads/bads/bads_dump.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/gaussian_process_train.py` & `PyBADS-1.0.1/pybads/bads/gaussian_process_train.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/optimize_result.py` & `PyBADS-1.0.1/pybads/bads/optimize_result.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/option_configs/advanced_bads_options.ini` & `PyBADS-1.0.1/pybads/bads/option_configs/advanced_bads_options.ini`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/option_configs/basic_bads_options.ini` & `PyBADS-1.0.1/pybads/bads/option_configs/basic_bads_options.ini`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/bads/options.py` & `PyBADS-1.0.1/pybads/bads/options.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/decorators/README.md` & `PyBADS-1.0.1/pybads/decorators/README.md`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/decorators/handle_0D_1D_input.py` & `PyBADS-1.0.1/pybads/decorators/handle_0D_1D_input.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/function_examples.py` & `PyBADS-1.0.1/pybads/function_examples.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/function_logger/constraints_check.py` & `PyBADS-1.0.1/pybads/function_logger/constraints_check.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/function_logger/function_logger.py` & `PyBADS-1.0.1/pybads/function_logger/function_logger.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/init_functions/init_sobol.py` & `PyBADS-1.0.1/pybads/init_functions/init_sobol.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/poll/poll_mads_2n.py` & `PyBADS-1.0.1/pybads/poll/poll_mads_2n.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/search/es_search.py` & `PyBADS-1.0.1/pybads/search/es_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,18 +306,14 @@
             - 0.5 * width_scaled[periodic_vars]
         )
         u_tmp[periodic_vars] = 0.0
 
     u_shift = U_tmp - u_tmp
 
     if w.size != 0:
-        weights = w.reshape(
-            -1, *[1] * U.shape[1]
-        )  # For broadcasting weighted sum
-        C = np.sum(weights * (u_shift.T @ u_shift), axis=0)
-        C = C.reshape(
-            (U.shape[1], U.shape[1])
-        )  # Remove the extra dimesion from the broadcast result
+        weights = w.reshape(-1, *([1] * u_shift.ndim))  # For broadcasting weighted sum
+        C = np.matmul(u_shift.transpose(), weights * u_shift)
+        C = np.sum(C, axis=0)
     else:
         C = u_shift.T @ u_shift
 
     return C
```

### Comparing `PyBADS-1.0.0/pybads/search/grid_functions.py` & `PyBADS-1.0.1/pybads/search/grid_functions.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/search/search_hedge.py` & `PyBADS-1.0.1/pybads/search/search_hedge.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/stats/get_hpd.py` & `PyBADS-1.0.1/pybads/stats/get_hpd.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/stats/kde1d.py` & `PyBADS-1.0.1/pybads/stats/kde1d.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/stats/kldiv_mvn.py` & `PyBADS-1.0.1/pybads/stats/kldiv_mvn.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/hyp.dat` & `PyBADS-1.0.1/pybads/testing/bads/hyp.dat`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/poll/test_poll_mads.py` & `PyBADS-1.0.1/pybads/testing/bads/poll/test_poll_mads.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/scripts/ackley_example.py` & `PyBADS-1.0.1/pybads/testing/bads/scripts/ackley_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py` & `PyBADS-1.0.1/pybads/testing/bads/scripts/bads_quadratic_noisy_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
 from pybads import BADS
 from pybads.bads import BADSDump
 from pybads.function_examples import quadratic_unknown_noisy_fcn, extra_noisy_quadratic_fcn, quadratic_hetsk_noisy_fcn, rosebrocks_hetsk_noisy_fcn
 
-x0 = np.array([[-3, -3]]);        # Starting point
-lb = np.array([[-5, -5]])     # Lower bounds
-ub = np.array([[5, 5]])       # Upper bounds
-plb = np.array([[-2, -2]])      # Plausible lower bounds
-pub = np.array([[2, 2]])        # Plausible upper bounds
+D = 3
+x0 = np.ones((1, D)) * -3      # Starting point
+lb = np.ones((1, D)) * -7      # Lower bounds
+ub = np.ones((1, D)) * 7       # Upper bounds
+plb = np.ones((1, D)) * -3     # Plausible lower bounds
+pub = np.ones((1, D)) * 3     # Plausible upper bounds
 
 title = 'Noise objective function'
 print("\n *** Example 3: " + title)
 print("\t We test BADS on a noisy quadratic function with unit Gaussian noise.")
 bads = BADS(quadratic_unknown_noisy_fcn, x0, lb, ub, plb, pub)
 
 optimize_result = bads.optimize()
```

### Comparing `PyBADS-1.0.0/pybads/testing/bads/scripts/bads_rosenbrock_example.py` & `PyBADS-1.0.1/pybads/testing/bads/scripts/bads_rosenbrock_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/scripts/non_bound_example.py` & `PyBADS-1.0.1/pybads/testing/bads/scripts/non_bound_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/scripts/rastrigin_example.py` & `PyBADS-1.0.1/pybads/testing/bads/scripts/rastrigin_example.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/search/test_search.py` & `PyBADS-1.0.1/pybads/testing/bads/search/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     # Starting point
     lb = np.array([[-20, -20, -20]])  # Lower bounds
     ub = np.array([[20, 20, 20]])  # Upper bounds
     plb = np.array([[-5, -5, -5]])  # Plausible lower bounds
     pub = np.array([[5, 5, 5]])  # Plausible upper bounds
     D = 3
     bads = BADS(rosenbrocks_fcn, x0, lb, ub, plb, pub)
-    bads.options["fun_eval_start"] = 0
+    bads.options["fun_eval_start"] = 10
     gp, Ns_gp, sn2hpd, hyp_dict = bads._init_optimization_()
 
     es_iter = bads.options["n_search_iter"]
     mu = int(bads.options["n_search"] / es_iter)
     lamb = mu
     search_es = ESSearchWM(mu, lamb, bads.options)
     us, z = search_es(
@@ -108,27 +108,26 @@
     lb = np.array([[-20, -20, -20]])  # Lower bounds
     ub = np.array([[20, 20, 20]])  # Upper bounds
     plb = np.array([[-5, -5, -5]])  # Plausible lower bounds
     pub = np.array([[5, 5, 5]])  # Plausible upper bounds
     D = 3
 
     bads = BADS(rosenbrocks_fcn, x0, lb, ub, plb, pub)
-    bads.options["fun_eval_start"] = 0
+    bads.options["fun_eval_start"] = 10
     gp, Ns_gp, sn2hpd, hyp_dict = bads._init_optimization_()
 
     search_hedge = ESSearchHedge(bads.options["search_method"], bads.options)
 
     us, z = search_hedge(
         bads.u, lb, ub, bads.function_logger, gp, bads.optim_state
     )
     print(search_hedge.chosen_search_fun)
     assert us.size == 3 and (np.isscalar(z) or z.size == 1)
     assert np.all(gp.y >= z)
 
-
 def test_u_cov():
     U = np.array(
         [
             [0, 0, 0],
             [0.1172, 0.1328, 0.6641],
             [0, 0, 1],
             [0, 0, -1],
@@ -138,26 +137,25 @@
     u0 = np.array([[0.0, 0.0, 0.0]])
     ub = np.array([[4.0, 4.0, 4.0]])
     lb = -ub
     w = np.array([0.4563, 0.2708, 0.1622, 0.0852, 0.0255])
     C = ucov(U, u0, w, ub, lb, 1)
     assert C.shape == (U.shape[1], U.shape[1])
 
-
 def test_grid_search_neighbors():
     x0 = np.array([[0, 0]])
     # Starting point
     lb = np.array([[-20, -20]])  # Lower bounds
     ub = np.array([[20, 20]])  # Upper bounds
     plb = np.array([[-5, -5]])  # Plausible lower bounds
     pub = np.array([[5, 5]])  # Plausible upper bounds
     D = 2
 
     bads = BADS(rosenbrocks_fcn, x0, lb, ub, plb, pub)
-    bads.options["fun_eval_start"] = 0
+    bads.options["fun_eval_start"] = 10
     gp, Ns_gp, sn2hpd, hyp_dict = bads._init_optimization_()
     gp.X = np.array([[0, 0], [-0.1055, 0.4570], [-0.3555, -0.7930]])
     f = FunctionLogger(rosenbrocks_fcn, D, False, 0)
     f.X = gp.X.copy()
     gp.y = np.array([1, 405.1637, 5.082e3])
     f.Y = gp.y.copy()
 
@@ -171,7 +169,8 @@
         f, np.array([[0, 0]]), gp, bads.options, bads.optim_state
     )[0]
     assert (
         result[0, 0] == 0.0
         and np.isclose(result[1, 0], -0.1055, 1e-3)
         and np.isclose(result[2, 0], -0.3555, 1e-3)
     )
+
```

### Comparing `PyBADS-1.0.0/pybads/testing/bads/test_bads_optimization.py` & `PyBADS-1.0.1/pybads/testing/bads/test_bads_optimization.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 import numpy as np
 import pytest
 from scipy.stats import norm
 
 from pybads.bads import BADS
 
 
-def get_test_opt_conf():
-    D = 3
+def get_test_opt_conf(D=3):
     x0 = np.ones((1, D)) * 4
     LB = -100*np.ones(D)                # Lower bound
     UB = 100*np.ones(D)                 # Upper bound
     PLB = -8*np.ones(D)                 # Plausible lower bound
     PUB = 12*np.ones(D)                 # Plausible upper bound
     tol_errs = np.array([0.1, 0.1, 1, 1.])
     return D, x0, LB, UB, PLB, PUB, tol_errs
 
 def run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min,
-            oracle_fun=None, non_box_cons=None, he_noise_flag=False,
-            assert_flag=False):
+            oracle_fun=None, non_box_cons=None, uncertainty_handling=False,
+            assert_flag=False, max_fun_evals=None):
     options = {}
     options["display"] = "full"#debug_flag = True
 
-    if he_noise_flag:
-        options["specify_target_noise"] = True
+    if uncertainty_handling > 0:
         options["uncertainty_handling"] = True
-        #options["noise_final_samples"] = 100
-        options["max_fun_evals"] = 200
+        options["max_fun_evals"] = 200 if max_fun_evals is None  else max_fun_evals
+        options["specify_target_noise"] = True
+        if uncertainty_handling > 1:
+            options["specify_target_noise"] = True
     else:
-        options["max_fun_evals"] = 100
+        options["max_fun_evals"] = 100 if max_fun_evals is None else max_fun_evals
 
     optimize_result = BADS(fun=fun, x0=x0, lower_bounds=LB,
                                     upper_bounds=UB, plausible_lower_bounds=PLB,
                                     plausible_upper_bounds=PUB, non_box_cons=non_box_cons,
                                     options=options).optimize()
     x = optimize_result['x']
     fval = optimize_result['fval']
@@ -43,19 +43,25 @@
     else:
         fval_true = oracle_fun(x)
         #print(f"Final value (not-noisy): {fval_true:.3f} (true value: {f_min}) with {optimize_result['func_count']} fun evals.")
         err = np.abs(fval_true - f_min)
     if assert_flag:
         assert np.any(err < tol_errs), f"Error {err} is not smaller than tolerance {tol_errs} when optimizing {fun.__name__}."
     
+    return optimize_result, err
+    
 def test_ellipsoid_opt():
     D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf()
     fun = lambda x: np.sum((np.atleast_2d(x) / np.arange(1, len(x) + 1) ** 2) ** 2)
     run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, assert_flag=True)
-    
+
+def test_high_dim_opt():
+    D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf(D=60)
+    fun = lambda x: np.sum((np.atleast_2d(x) / np.arange(1, len(x) + 1) ** 2) ** 2)
+    run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, assert_flag=False, max_fun_evals=200)
 
 def test_sphere_opt():
     D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf()
     x0 = np.zeros((1, D))
     fun = lambda x: np.sum(np.atleast_2d(x)**2, axis=1)
     non_box_cons = lambda x: np.atleast_2d(x)[:, 0] + np.atleast_2d(x)[:, 1] >= np.sqrt(2)     # Non-bound constraints
     print(non_box_cons(x0))
@@ -73,8 +79,8 @@
     y = y + s*np.random.randn()
     return y, s
 
 def test_he_noisy_sphere_opt():
     D, x0, LB, UB, PLB, PUB, tol_errs = get_test_opt_conf()
     fun = he_noisy_sphere
     oracle_fun = lambda x: np.sum(np.atleast_2d(x)**2, axis=1)                          # True objective function
-    run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, oracle_fun=oracle_fun, he_noise_flag=True, assert_flag=True)
+    run_bads(fun, x0, LB, UB, PLB, PUB, tol_errs, f_min=0.0, oracle_fun=oracle_fun, uncertainty_handling=2, assert_flag=True)
```

### Comparing `PyBADS-1.0.0/pybads/testing/bads/test_gaussian_process_train.py` & `PyBADS-1.0.1/pybads/testing/bads/test_gaussian_process_train.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/bads/test_iteration_history.py` & `PyBADS-1.0.1/pybads/testing/bads/test_iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py` & `PyBADS-1.0.1/pybads/testing/decorators/test_handle_0D_1D_input_decorator.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/function_logger/test_function_logger.py` & `PyBADS-1.0.1/pybads/testing/function_logger/test_function_logger.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/testing/variable_transformer/test_variable_transformer.py` & `PyBADS-1.0.1/pybads/testing/variable_transformer/test_variable_transformer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/utils/iteration_history.py` & `PyBADS-1.0.1/pybads/utils/iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/utils/timer/timer.py` & `PyBADS-1.0.1/pybads/utils/timer/timer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pybads/variable_transformer/variables_transformer.py` & `PyBADS-1.0.1/pybads/variable_transformer/variables_transformer.py`

 * *Files identical despite different names*

### Comparing `PyBADS-1.0.0/pyproject.toml` & `PyBADS-1.0.1/pyproject.toml`

 * *Files identical despite different names*

