# Comparing `tmp/qlknn-1.2.1.tar.gz` & `tmp/qlknn-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlknn-1.2.1.tar", last modified: Wed Aug 31 13:01:17 2022, max compression
+gzip compressed data, was "qlknn-1.3.1.tar", max compression
```

## Comparing `qlknn-1.2.1.tar` & `qlknn-1.3.1.tar`

### file list

```diff
@@ -1,287 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.147297 qlknn-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-08-31 13:01:04.000000 qlknn-1.2.1/.git-blame-ignore-revs
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-08-31 13:01:04.000000 qlknn-1.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     7480 2022-08-31 13:01:04.000000 qlknn-1.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     1109 2022-08-31 13:01:04.000000 qlknn-1.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2896 2022-08-31 13:01:04.000000 qlknn-1.2.1/Makefile
--rw-r--r--   0 root         (0) root         (0)      992 2022-08-31 13:01:17.147297 qlknn-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      249 2022-08-31 13:01:04.000000 qlknn-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.030286 qlknn-1.2.1/doc/
--rw-rw-rw-   0 root         (0) root         (0)       11 2022-08-31 13:01:04.000000 qlknn-1.2.1/doc/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.031286 qlknn-1.2.1/doc/yed/
--rw-rw-rw-   0 root         (0) root         (0)   185768 2022-08-31 13:01:04.000000 qlknn-1.2.1/doc/yed/filtering.graphml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.032287 qlknn-1.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1514 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.034287 qlknn-1.2.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.035287 qlknn-1.2.1/docs/source/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.037287 qlknn-1.2.1/docs/source/_templates/autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      172 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/autosummary/accessor.rst
--rw-rw-rw-   0 root         (0) root         (0)      181 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/autosummary/accessor_attribute.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/autosummary/accessor_callable.rst
--rw-rw-rw-   0 root         (0) root         (0)      178 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/autosummary/accessor_method.rst
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/autosummary/base.rst
--rw-rw-rw-   0 root         (0) root         (0)      611 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/custom-class-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     1219 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/custom-module-template.rst
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/_templates/layout.html
--rw-rw-rw-   0 root         (0) root         (0)      547 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/api-hidden.rst
--rw-rw-rw-   0 root         (0) root         (0)      883 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/api.rst
--rw-rw-rw-   0 root         (0) root         (0)    18550 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1162 2022-08-31 13:01:04.000000 qlknn-1.2.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.011284 qlknn-1.2.1/envs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.038287 qlknn-1.2.1/envs/docker-python/
--rwxrwxrwx   0 root         (0) root         (0)     1837 2022-08-31 13:01:04.000000 qlknn-1.2.1/envs/docker-python/00_prepare_venv_path.sh
--rwxrwxrwx   0 root         (0) root         (0)      110 2022-08-31 13:01:04.000000 qlknn-1.2.1/envs/docker-python/20_setenv_pure_python.sh
--rwxrwxrwx   0 root         (0) root         (0)      802 2022-08-31 13:01:04.000000 qlknn-1.2.1/envs/docker-python/21_activate_python_venv.sh
--rwxrwxrwx   0 root         (0) root         (0)      136 2022-08-31 13:01:04.000000 qlknn-1.2.1/envs/docker-python/22_install_qualikiz_tools.sh
--rw-rw-rw-   0 root         (0) root         (0)      272 2022-08-31 13:01:04.000000 qlknn-1.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      724 2022-08-31 13:01:04.000000 qlknn-1.2.1/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.039287 qlknn-1.2.1/qlknn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.043287 qlknn-1.2.1/qlknn/NNDB/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/NNDB/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/NNDB/extract_nns.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/NNDB/get_best.py
--rw-rw-rw-   0 root         (0) root         (0)    66861 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/NNDB/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/NNDB/postprocess.py
--rw-rw-rw-   0 root         (0) root         (0)     7364 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/NNDB/stats.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.047288 qlknn-1.2.1/qlknn/dataset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5605 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/calculate_instance_weights.py
--rw-rw-rw-   0 root         (0) root         (0)    18545 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/clustering.py
--rw-rw-rw-   0 root         (0) root         (0)    18243 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/data_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.050288 qlknn-1.2.1/qlknn/dataset/filter_archive/
--rw-rw-rw-   0 root         (0) root         (0)    13880 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_eight.py
--rw-rw-rw-   0 root         (0) root         (0)     2259 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_eight_glueing.py
--rw-rw-rw-   0 root         (0) root         (0)     2259 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_eight_output_statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_seven.py
--rw-rw-rw-   0 root         (0) root         (0)     6420 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_six.py
--rw-rw-rw-   0 root         (0) root         (0)     6881 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/megarun_one_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10579 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_archive/megarun_one_to_pandas.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filter_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)    34259 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/filtering.py
--rw-rw-rw-   0 root         (0) root         (0)    22153 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/hypercube_to_pandas.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     6531 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/prep_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/dataset/separate7D.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.050288 qlknn-1.2.1/qlknn/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/gui/slice_gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.054288 qlknn-1.2.1/qlknn/misc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/activation_showcase.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/analyse_names.py
--rw-rw-rw-   0 root         (0) root         (0)     4099 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/binning.py
--rwxrwxrwx   0 root         (0) root         (0)     3063 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/dataset_measure_mem.sh
--rw-rw-rw-   0 root         (0) root         (0)     1327 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/dataset_memtest.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/dataset_snippits.py
--rw-rw-rw-   0 root         (0) root         (0)     6750 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/dataset_storage_format_profiler.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/get_dataset_standardization.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/random_access_benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)     9810 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/to_precision.py
--rw-rw-rw-   0 root         (0) root         (0)     4809 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/misc/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.059289 qlknn-1.2.1/qlknn/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5415 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/clipping.py
--rw-rw-rw-   0 root         (0) root         (0)    18583 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/committee.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/cython_mkl_ndnn.py
--rw-rw-rw-   0 root         (0) root         (0)    26130 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/ffnn.py
--rw-rw-rw-   0 root         (0) root         (0)    46428 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/kerasmodel.py
--rw-rw-rw-   0 root         (0) root         (0)    10536 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/qlknn_fortran.py
--rw-rw-rw-   0 root         (0) root         (0)     5856 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/qlknn_hyper_10D.py
--rw-rw-rw-   0 root         (0) root         (0)    15260 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/qlknnmodule.c
--rw-rw-rw-   0 root         (0) root         (0)     5872 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/rotdiv.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    15878 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/models/victor_rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.062289 qlknn-1.2.1/qlknn/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/luigi.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2872 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/one_off_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    21544 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/simple_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/train_NDNN_cori_haswell.sh
--rwxrwxrwx   0 root         (0) root         (0)      353 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/train_NDNN_lisa.sh
--rwxrwxrwx   0 root         (0) root         (0)     1020 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/train_NDNN_marconi.sh
--rw-rw-rw-   0 root         (0) root         (0)     2432 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/pipeline/train_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.067290 qlknn-1.2.1/qlknn/plots/
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     6644 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/HornNet_slice.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.069290 qlknn-1.2.1/qlknn/plots/comparison/
--rw-rw-rw-   0 root         (0) root         (0)     2266 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/early_stop.py
--rw-rw-rw-   0 root         (0) root         (0)     2237 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2241 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/goodness.py
--rw-rw-rw-   0 root         (0) root         (0)     1517 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/query_to_networks.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/regularization.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/similarity.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/comparison/topology.py
--rwxrwxrwx   0 root         (0) root         (0)      965 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/default_settings_HornNet_slice.json
--rw-rw-rw-   0 root         (0) root         (0)     4340 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/error_heatmap.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/hyperpar_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     3568 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/load_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4732 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/measures_of_goodness.py
--rw-rw-rw-   0 root         (0) root         (0)     1621 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/plot_camille_NNs.py
--rw-rw-rw-   0 root         (0) root         (0)     5663 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/plot_nn_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     7204 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/popplots.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/qlk_slice_plot_camille.py
--rw-rw-rw-   0 root         (0) root         (0)    65054 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/quickslicer.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/quickslicer_dummy_net.py
--rw-rw-rw-   0 root         (0) root         (0)     3317 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/plots/statistical_spread.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/setup_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.074290 qlknn-1.2.1/qlknn/training/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13955 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/default_settings.json
--rw-rw-rw-   0 root         (0) root         (0)     1873 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/edgerun8_settings.json
--rw-rw-rw-   0 root         (0) root         (0)     1897 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/gridSearch.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/gridSearch_structure.py
--rw-rw-rw-   0 root         (0) root         (0)    14753 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/keras_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    44660 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/keras_models.py
--rw-rw-rw-   0 root         (0) root         (0)    12532 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/nn_primitives.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/train_NDNN.py
--rwxrwxrwx   0 root         (0) root         (0)     5866 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/train_NDNN_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    38896 2022-08-31 13:01:04.000000 qlknn-1.2.1/qlknn/training/train_NDNN_legacy.py
--rw-r--r--   0 root         (0) root         (0)        7 2022-08-31 13:01:16.000000 qlknn-1.2.1/qlknn/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.041287 qlknn-1.2.1/qlknn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      992 2022-08-31 13:01:16.000000 qlknn-1.2.1/qlknn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8539 2022-08-31 13:01:17.000000 qlknn-1.2.1/qlknn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-31 13:01:16.000000 qlknn-1.2.1/qlknn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2022-08-31 13:01:16.000000 qlknn-1.2.1/qlknn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      580 2022-08-31 13:01:16.000000 qlknn-1.2.1/qlknn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-08-31 13:01:16.000000 qlknn-1.2.1/qlknn.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_core.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_dataset.txt
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_docs.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_gui.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_nndb.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_pipeline.txt
--rw-rw-rw-   0 root         (0) root         (0)       27 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-08-31 13:01:04.000000 qlknn-1.2.1/requirements_training.txt
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-08-31 13:01:17.147297 qlknn-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3848 2022-08-31 13:01:04.000000 qlknn-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.021285 qlknn-1.2.1/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.075290 qlknn-1.2.1/testdata/clustering/
--rw-rw-rw-   0 root         (0) root         (0)      392 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/clustering/settings_DBMSND.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.016285 qlknn-1.2.1/testdata/committee_nets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.016285 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.077291 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_0/
--rw-rw-rw-   0 root         (0) root         (0)  1126094 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_0/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_0/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.079291 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_1/
--rw-rw-rw-   0 root         (0) root         (0)  1126013 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_1/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_1/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.081291 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_2/
--rw-rw-rw-   0 root         (0) root         (0)  1125981 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_2/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_2/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.084291 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_3/
--rw-rw-rw-   0 root         (0) root         (0)  1125931 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_3/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_3/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.086291 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_4/
--rw-rw-rw-   0 root         (0) root         (0)  1126131 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_4/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efeTEM_GB/NN_4/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.018285 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.088292 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_0/
--rw-rw-rw-   0 root         (0) root         (0)  1126052 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_0/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_0/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.090292 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_1/
--rw-rw-rw-   0 root         (0) root         (0)  1125752 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_1/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_1/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.092292 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_2/
--rw-rw-rw-   0 root         (0) root         (0)  1125967 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_2/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_2/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.094292 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_3/
--rw-rw-rw-   0 root         (0) root         (0)  1126162 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_3/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_3/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.096292 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_4/
--rw-rw-rw-   0 root         (0) root         (0)  1126248 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_4/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     2018 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/committee_nets/Cmte_efiITG_GB/NN_4/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.102293 qlknn-1.2.1/testdata/gen2_test_files/
--rw-rw-rw-   0 root         (0) root         (0)  3008608 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/4D_nions0_flat.h5
--rw-rw-rw-   0 root         (0) root         (0)    12757 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/filtering.py
--rw-rw-rw-   0 root         (0) root         (0)     4476 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/hypercube_to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.109294 qlknn-1.2.1/testdata/gen2_test_files/network_1393/
--rw-rw-rw-   0 root         (0) root         (0)   726571 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/network_1393/nn.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/network_1393/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/network_1393/train_NDNN.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.111294 qlknn-1.2.1/testdata/gen2_test_files/network_1440/
--rw-rw-rw-   0 root         (0) root         (0)   719985 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/network_1440/nn.json
--rw-rw-rw-   0 root         (0) root         (0)      957 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/network_1440/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/network_1440/train_NDNN.py
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/train_NDNN.py
--rw-rw-rw-   0 root         (0) root         (0)  4776988 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen2_test_files/unstable_training_gen2_4D_nions0_flat_filter8.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.112294 qlknn-1.2.1/testdata/gen3_test_files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.115294 qlknn-1.2.1/testdata/gen3_test_files/Network_302_efeITG_GB_div_efiITG_GB/
--rw-rw-rw-   0 root         (0) root         (0)  1147832 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_302_efeITG_GB_div_efiITG_GB/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1173 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_302_efeITG_GB_div_efiITG_GB/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_302_efeITG_GB_div_efiITG_GB/train_NDNN.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.118294 qlknn-1.2.1/testdata/gen3_test_files/Network_591_efeTEM_GB/
--rw-rw-rw-   0 root         (0) root         (0)  1156998 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_591_efeTEM_GB/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1157 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_591_efeTEM_GB/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_591_efeTEM_GB/train_NDNN.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.120295 qlknn-1.2.1/testdata/gen3_test_files/Network_711_gam_leq_GB/
--rw-rw-rw-   0 root         (0) root         (0)  1164860 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_711_gam_leq_GB/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1163 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_711_gam_leq_GB/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_711_gam_leq_GB/train_NDNN.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.123295 qlknn-1.2.1/testdata/gen3_test_files/Network_874_efiITG_GB/
--rw-rw-rw-   0 root         (0) root         (0)  1153962 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_874_efiITG_GB/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1148 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_874_efiITG_GB/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    27676 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/Network_874_efiITG_GB/train_NDNN.py
--rw-rw-rw-   0 root         (0) root         (0)   969974 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen3_test_files/unstable_training_gen3_4D_nions0_flat_filter8.h5.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.123295 qlknn-1.2.1/testdata/gen4_test_files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.126295 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efeITG_GB_div_efiITG_GB/
--rw-rw-rw-   0 root         (0) root         (0)  1163966 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efeITG_GB_div_efiITG_GB/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1420 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efeITG_GB_div_efiITG_GB/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    37799 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efeITG_GB_div_efiITG_GB/train_NDNN.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.128295 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB/
--rw-rw-rw-   0 root         (0) root         (0)  1156684 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1406 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    37799 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB/train_NDNN.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.131296 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB_div_efiITG_GB_rot0/
--rw-rw-rw-   0 root         (0) root         (0)  1174335 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB_div_efiITG_GB_rot0/nn.json
--rw-rw-rw-   0 root         (0) root         (0)     1442 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB_div_efiITG_GB_rot0/settings.json
--rw-rw-rw-   0 root         (0) root         (0)    35709 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/Network_xxx_efiITG_GB_div_efiITG_GB_rot0/train_NDNN.py
--rw-rw-rw-   0 root         (0) root         (0)    24003 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/filtering.py
--rw-rw-rw-   0 root         (0) root         (0)    18565 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen4_test_files/hypercube_to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.131296 qlknn-1.2.1/testdata/gen5_test_files/
--rw-rw-rw-   0 root         (0) root         (0)  3129495 2022-08-31 13:01:04.000000 qlknn-1.2.1/testdata/gen5_test_files/gen5_4D_nions0_flat_filter10.h5.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.136296 qlknn-1.2.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.137296 qlknn-1.2.1/tests/NNDB/
--rw-rw-rw-   0 root         (0) root         (0)     3263 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/NNDB/base.py
--rw-rw-rw-   0 root         (0) root         (0)    27777 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/NNDB/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/NNDB/test_postprocess.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11768 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.138296 qlknn-1.2.1/tests/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     1826 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/dataset/test_clustering.py
--rw-rw-rw-   0 root         (0) root         (0)     2820 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/dataset/test_data_io.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/dataset/test_filtering.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/dataset/test_hypercube_to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.142297 qlknn-1.2.1/tests/keras_test_files/
--rw-rw-rw-   0 root         (0) root         (0)     6795 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/keras_test_files/philippstyle_CGNN_inp.csv
--rw-rw-rw-   0 root         (0) root         (0)    30485 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/keras_test_files/philippstyle_CGNN_model.json
--rw-rw-rw-   0 root         (0) root         (0)     3106 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/keras_test_files/philippstyle_CGNN_outp.csv
--rw-rw-rw-   0 root         (0) root         (0)  1506789 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/keras_test_files/philippstyle_CGNN_weights.json
--rw-rw-rw-   0 root         (0) root         (0)      506 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/keras_test_files/training_gen3_7D_nions0_flat_filter8.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.142297 qlknn-1.2.1/tests/misc/
--rw-rw-rw-   0 root         (0) root         (0)    12612 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/misc/test_analyse_names.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.143297 qlknn-1.2.1/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)     1846 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/models/test_committee.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/models/test_ffnn.py
--rw-rw-rw-   0 root         (0) root         (0)     2259 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/models/test_kerasmodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.144297 qlknn-1.2.1/tests/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)     1338 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/pipeline/test_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.145297 qlknn-1.2.1/tests/plots/
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/plots/test_load_data.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/plots/test_measures_of_goodness.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/plots/test_popplots.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/plots/test_quickslicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:01:17.146297 qlknn-1.2.1/tests/training/
--rw-rw-rw-   0 root         (0) root         (0)     1748 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/training/test_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     9328 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/training/test_keras_models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/training/test_nn_primitives.py
--rw-rw-rw-   0 root         (0) root         (0)     3746 2022-08-31 13:01:04.000000 qlknn-1.2.1/tests/training/test_train_NDNN.py
+-rw-r--r--   0        0        0     1109 2022-12-14 15:03:50.264825 qlknn-1.3.1/LICENSE
+-rw-r--r--   0        0        0      249 2022-12-14 15:03:50.264825 qlknn-1.3.1/README.md
+-rw-r--r--   0        0        0     1941 2023-07-13 10:13:12.686764 qlknn-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/NNDB/__init__.py
+-rw-r--r--   0        0        0     2246 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/NNDB/extract_nns.py
+-rw-r--r--   0        0        0     2002 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/NNDB/get_best.py
+-rw-r--r--   0        0        0    66861 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/NNDB/model.py
+-rw-r--r--   0        0        0     3900 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/NNDB/postprocess.py
+-rw-r--r--   0        0        0     7364 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/NNDB/stats.py
+-rw-r--r--   0        0        0      615 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/__init__.py
+-rw-r--r--   0        0        0     1727 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/cli.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/dataset/__init__.py
+-rw-r--r--   0        0        0     5605 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/calculate_instance_weights.py
+-rw-r--r--   0        0        0    18545 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/clustering.py
+-rw-r--r--   0        0        0    18243 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/data_io.py
+-rw-r--r--   0        0        0    13880 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_eight.py
+-rw-r--r--   0        0        0     2259 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_eight_glueing.py
+-rw-r--r--   0        0        0     2259 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_eight_output_statistics.py
+-rw-r--r--   0        0        0     5641 2022-12-14 15:03:50.268158 qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_seven.py
+-rw-r--r--   0        0        0     6420 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_six.py
+-rw-r--r--   0        0        0    15605 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_ten.py
+-rw-r--r--   0        0        0     6881 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/filter_archive/megarun_one_filter.py
+-rw-r--r--   0        0        0    10579 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/filter_archive/megarun_one_to_pandas.py
+-rw-r--r--   0        0        0     2469 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/filter_datasets.py
+-rw-r--r--   0        0        0    34272 2023-07-12 14:27:47.224809 qlknn-1.3.1/qlknn/dataset/filtering.py
+-rw-r--r--   0        0        0    22264 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/hypercube_to_pandas.py
+-rw-r--r--   0        0        0     1834 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/mapping.py
+-rw-r--r--   0        0        0     6531 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/prep_datasets.py
+-rw-r--r--   0        0        0     1425 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/dataset/separate7D.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/gui/__init__.py
+-rw-r--r--   0        0        0     4555 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/gui/slice_gui.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/misc/__init__.py
+-rw-r--r--   0        0        0     1058 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/activation_showcase.py
+-rw-r--r--   0        0        0    11583 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/analyse_names.py
+-rw-r--r--   0        0        0     4099 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/binning.py
+-rwxr-xr-x   0        0        0     3063 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/dataset_measure_mem.sh
+-rw-r--r--   0        0        0     1327 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/dataset_memtest.py
+-rw-r--r--   0        0        0     2838 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/dataset_snippits.py
+-rw-r--r--   0        0        0     6750 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/dataset_storage_format_profiler.py
+-rw-r--r--   0        0        0      525 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/get_dataset_standardization.py
+-rw-r--r--   0        0        0     3952 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/random_access_benchmark.py
+-rw-r--r--   0        0        0     9810 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/misc/to_precision.py
+-rw-r--r--   0        0        0     4807 2023-07-12 14:27:47.224809 qlknn-1.3.1/qlknn/misc/tools.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/models/__init__.py
+-rw-r--r--   0        0        0     5415 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/models/clipping.py
+-rw-r--r--   0        0        0    18721 2023-07-12 14:27:47.224809 qlknn-1.3.1/qlknn/models/committee.py
+-rw-r--r--   0        0        0     2593 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/models/cython_mkl_ndnn.py
+-rw-r--r--   0        0        0    26421 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/models/ffnn.py
+-rw-r--r--   0        0        0    46428 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/models/kerasmodel.py
+-rw-r--r--   0        0        0    10536 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/models/qlknn_fortran.py
+-rw-r--r--   0        0        0     5856 2022-12-14 15:03:50.271491 qlknn-1.3.1/qlknn/models/qlknn_hyper_10D.py
+-rw-r--r--   0        0        0    15260 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/models/qlknnmodule.c
+-rw-r--r--   0        0        0     5872 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/models/rotdiv.py
+-rw-r--r--   0        0        0     1703 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/models/setup.py
+-rw-r--r--   0        0        0    15878 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/models/victor_rule.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/pipeline/__init__.py
+-rw-r--r--   0        0        0      345 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/luigi.cfg
+-rw-r--r--   0        0        0     2872 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/one_off_tasks.py
+-rw-r--r--   0        0        0    21544 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/pipeline.py
+-rw-r--r--   0        0        0     1150 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/simple_scanner.py
+-rw-r--r--   0        0        0      340 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/train_NDNN_cori_haswell.sh
+-rwxr-xr-x   0        0        0      353 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/train_NDNN_lisa.sh
+-rwxr-xr-x   0        0        0     1020 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/train_NDNN_marconi.sh
+-rw-r--r--   0        0        0     2432 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/pipeline/train_launch.py
+-rw-r--r--   0        0        0        6 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/.gitignore
+-rw-r--r--   0        0        0     6644 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/HornNet_slice.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/plots/__init__.py
+-rw-r--r--   0        0        0     2266 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/early_stop.py
+-rw-r--r--   0        0        0     2237 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/filter.py
+-rw-r--r--   0        0        0     2241 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/goodness.py
+-rw-r--r--   0        0        0     1517 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/query_to_networks.py
+-rw-r--r--   0        0        0     2561 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/regularization.py
+-rw-r--r--   0        0        0     2149 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/similarity.py
+-rw-r--r--   0        0        0     2796 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/comparison/topology.py
+-rwxr-xr-x   0        0        0      965 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/default_settings_HornNet_slice.json
+-rw-r--r--   0        0        0     4340 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/error_heatmap.py
+-rw-r--r--   0        0        0     5370 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/hyperpar_scan.py
+-rw-r--r--   0        0        0     3568 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/load_data.py
+-rw-r--r--   0        0        0     5207 2023-07-12 14:27:47.228142 qlknn-1.3.1/qlknn/plots/measures_of_goodness.py
+-rw-r--r--   0        0        0     1621 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/plot_camille_NNs.py
+-rw-r--r--   0        0        0     5663 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/plot_nn_structure.py
+-rw-r--r--   0        0        0     7204 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/popplots.py
+-rw-r--r--   0        0        0      704 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/qlk_slice_plot_camille.py
+-rw-r--r--   0        0        0    70259 2023-07-13 10:12:41.410868 qlknn-1.3.1/qlknn/plots/quickslicer.py
+-rw-r--r--   0        0        0     2443 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/quickslicer_dummy_net.py
+-rw-r--r--   0        0        0     3317 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/plots/statistical_spread.py
+-rw-r--r--   0        0        0     2121 2022-12-14 15:03:50.274825 qlknn-1.3.1/qlknn/setup_logging.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:12:41.650862 qlknn-1.3.1/qlknn/training/__init__.py
+-rw-r--r--   0        0        0    13955 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/datasets.py
+-rw-r--r--   0        0        0     1926 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/default_settings.json
+-rw-r--r--   0        0        0     1873 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/edgerun8_settings.json
+-rw-r--r--   0        0        0     1897 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/gridSearch.py
+-rw-r--r--   0        0        0     1921 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/gridSearch_structure.py
+-rw-r--r--   0        0        0    14753 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/keras_helpers.py
+-rw-r--r--   0        0        0    44660 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/keras_models.py
+-rw-r--r--   0        0        0    12532 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/nn_primitives.py
+-rw-r--r--   0        0        0      836 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/profiling.py
+-rw-r--r--   0        0        0     6309 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/train_NDNN.py
+-rwxr-xr-x   0        0        0     5866 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/train_NDNN_cli.py
+-rw-r--r--   0        0        0    38896 2022-12-14 15:03:50.278158 qlknn-1.3.1/qlknn/training/train_NDNN_legacy.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 qlknn-1.3.1/PKG-INFO
```

### Comparing `qlknn-1.2.1/LICENSE` & `qlknn-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/NNDB/extract_nns.py` & `qlknn-1.3.1/qlknn/NNDB/extract_nns.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/NNDB/get_best.py` & `qlknn-1.3.1/qlknn/NNDB/get_best.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/NNDB/model.py` & `qlknn-1.3.1/qlknn/NNDB/model.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/NNDB/postprocess.py` & `qlknn-1.3.1/qlknn/NNDB/postprocess.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/NNDB/stats.py` & `qlknn-1.3.1/qlknn/NNDB/stats.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/__init__.py` & `qlknn-1.3.1/qlknn/__init__.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/cli.py` & `qlknn-1.3.1/qlknn/cli.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/calculate_instance_weights.py` & `qlknn-1.3.1/qlknn/dataset/calculate_instance_weights.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/clustering.py` & `qlknn-1.3.1/qlknn/dataset/clustering.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/data_io.py` & `qlknn-1.3.1/qlknn/dataset/data_io.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_eight.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_eight.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_eight_glueing.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_eight_glueing.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_eight_output_statistics.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_eight_output_statistics.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_seven.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_seven.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/edgerun_six.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/edgerun_six.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/megarun_one_filter.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/megarun_one_filter.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_archive/megarun_one_to_pandas.py` & `qlknn-1.3.1/qlknn/dataset/filter_archive/megarun_one_to_pandas.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filter_datasets.py` & `qlknn-1.3.1/qlknn/dataset/filter_datasets.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/filtering.py` & `qlknn-1.3.1/qlknn/dataset/filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
             logger.debug("Applying functional filter")
             data = data.loc[cke_filter(data, cke_bound)]
         else:
             logger.debug("Applying stored filter")
             data = data.reindex(index=data.index.difference(stored_cke_filter), copy=False)
         if startlen is not None:
             logger.info(
-                "After filter {!s:<13} {:.f}% left".format("cke", 100 * len(data) / startlen)
+                "After filter {!s:<13} {:6.2f}% left".format("cke", 100 * len(data) / startlen)
             )
         else:
             logger.info("filter {!s:<13} done".format("cke"))
         gc.collect()
 
     if np.isfinite(cki_bound):
         # Throw away point if cki too high
@@ -940,15 +940,15 @@
         )
         save_to_store(inputs[dim], data.loc[idx[dim]], consts[dim], store_name, compress=compress)
 
 
 @profile
 def generate_test_train_index(input, data, const, frac=0.1):
     """Randomly split full dataset in 'test' and 'training' and save to store"""
-    rand_index = pd.Int64Index(np.random.permutation(input.index.copy(deep=True)))
+    rand_index = pd.Index(np.random.permutation(input.index.copy(deep=True)), dtype=np.int64)
     sep_index = int(frac * len(rand_index))
     # idx = {}
     # idx['test'] = rand_index[:sep_index]
     # idx['training'] = rand_index[sep_index:]
     data["is_test"] = False
     data.loc[rand_index[:sep_index], "is_test"] = True
```

### Comparing `qlknn-1.2.1/qlknn/dataset/hypercube_to_pandas.py` & `qlknn-1.3.1/qlknn/dataset/hypercube_to_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 from itertools import product
 import gc
 import os
 import copy
 import shutil
 import logging
+from pathlib import Path
 
 import numpy as np
 import xarray as xr
 import pandas as pd
 
 # from dask.distributed import Client, get_client
 parquet_engine = "pyarrow"
@@ -205,14 +206,17 @@
     """Determine the on-disk chunk sizes and open dataset
 
     Best performance in Dask is achieved if the on-disk chunks
     (as saved by xarray) are aligned with the Dask chunks.
     This function assumes all variables are chunked have the
     same on-disk chunks (the xarray default)
     """
+    path = Path(path)
+    if not path.exists():
+        raise FileNotFoundError(path)
     ds = xr.open_dataset(path)
     if dask:
         if base_chunk_var in ds.data_vars:
             chunk_sizes = ds[base_chunk_var]._variable._encoding["chunksizes"]
             dims = ds[base_chunk_var]._variable.dims
         else:
             raise Exception(
```

### Comparing `qlknn-1.2.1/qlknn/dataset/mapping.py` & `qlknn-1.3.1/qlknn/dataset/mapping.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/prep_datasets.py` & `qlknn-1.3.1/qlknn/dataset/prep_datasets.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/dataset/separate7D.py` & `qlknn-1.3.1/qlknn/dataset/separate7D.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/gui/slice_gui.py` & `qlknn-1.3.1/qlknn/gui/slice_gui.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/activation_showcase.py` & `qlknn-1.3.1/qlknn/misc/activation_showcase.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/analyse_names.py` & `qlknn-1.3.1/qlknn/misc/analyse_names.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/binning.py` & `qlknn-1.3.1/qlknn/misc/binning.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/dataset_measure_mem.sh` & `qlknn-1.3.1/qlknn/misc/dataset_measure_mem.sh`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/dataset_memtest.py` & `qlknn-1.3.1/qlknn/misc/dataset_memtest.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/dataset_snippits.py` & `qlknn-1.3.1/qlknn/misc/dataset_snippits.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/dataset_storage_format_profiler.py` & `qlknn-1.3.1/qlknn/misc/dataset_storage_format_profiler.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/get_dataset_standardization.py` & `qlknn-1.3.1/qlknn/misc/get_dataset_standardization.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/random_access_benchmark.py` & `qlknn-1.3.1/qlknn/misc/random_access_benchmark.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/to_precision.py` & `qlknn-1.3.1/qlknn/misc/to_precision.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/misc/tools.py` & `qlknn-1.3.1/qlknn/misc/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,11 +142,11 @@
                 log_func("qlknn is version {!s}".format(commit_sha[:8] + "-dirty"))
             else:
                 log_func("qlknn is version {!s}".format(commit_sha[:8]))
 
 
 def dataframe_okay(df: pd.DataFrame):
     """Checks if the pd.DataFrame s do not have NaNs, Nulls, and Infs."""
-    with pd.option_context("mode.use_inf_as_null", True):
+    with pd.option_context("mode.use_inf_as_na", True):
         is_not_null = df.isnull().sum().sum() == 0
         is_not_na = df.isna().sum().sum() == 0
     return is_not_null and is_not_na
```

### Comparing `qlknn-1.2.1/qlknn/models/clipping.py` & `qlknn-1.3.1/qlknn/models/clipping.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/committee.py` & `qlknn-1.3.1/qlknn/models/committee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import numpy as np
 import pandas as pd
+from pandas import Series
 from IPython import embed
 
 from qlknn.models.ffnn import QuaLiKizNDNN, QuaLiKizComboNN, determine_settings
 from qlknn.misc.analyse_names import is_pure_flux, is_flux, split_parts
 
 
 class QuaLiKizCommitteeNN(QuaLiKizNDNN):
@@ -114,48 +115,47 @@
                 feature_min = nn._feature_min.combine(feature_min, max)
         return feature_min
 
     @property
     def _target_names(self):
         names = None
         if len(self._nns) > 0:
-            names = self._nns[0]._target_names
-            eb_names = pd.Series([name + "_EB" for name in self._nns[0]._target_names])
-            names = names.append(eb_names)
-            names = names.reset_index(drop=True)
+            names: Series = self._nns[0]._target_names
+            eb_names: Series = pd.Series([name + "_EB" for name in self._nns[0]._target_names])
+            names = pd.concat([names, eb_names]).reset_index(drop=True)
         return names
 
     @property
     def _target_max(self):
         target_max = None
         if len(self._nns) > 0:
             eb_names = pd.Series([name + "_EB" for name in self._nns[0]._target_names])
             target_max = pd.Series(
                 np.full_like(self._nns[0]._target_max, np.inf),
                 index=self._nns[0]._target_max.index,
             )
             for nn in self._nns:
                 target_max = nn._target_max.combine(target_max, min)
             eb_max = pd.Series([np.inf] * len(eb_names), index=eb_names)
-            target_max = target_max.append(eb_max)
+            target_max = pd.concat([target_max, eb_max]).reset_index(drop=True)
         return target_max
 
     @property
     def _target_min(self):
         target_min = None
         if len(self._nns) > 0:
             eb_names = pd.Series([name + "_EB" for name in self._nns[0]._target_names])
             target_min = pd.Series(
                 np.full_like(self._nns[0]._target_min, -np.inf),
                 index=self._nns[0]._target_min.index,
             )
             for nn in self._nns:
                 target_min = nn._target_min.combine(target_min, max)
             eb_min = pd.Series([-np.inf] * len(eb_names), index=eb_names)
-            target_min = target_min.append(eb_min)
+            target_min = pd.concat([target_min, eb_min]).reset_index(drop=True)
         return target_min
 
     @property
     def _base_target_names(self):
         return self._nns[0]._target_names
 
 
@@ -419,15 +419,15 @@
             output = np.hstack(outlist)
         return output
 
     @property
     def _feature_names(self):
         feature_names = pd.Series()
         for nn in self._nns:
-            feature_names = feature_names.append(nn._feature_names)
+            feature_names = pd.concat([feature_names, nn._feature_names]).reset_index(drop=True)
         feature_names = pd.Series(feature_names.unique())
         return feature_names
 
     @property
     def _feature_max(self):
         feature_max = pd.Series(
             np.full_like(self._nns[0]._feature_max, np.inf),
@@ -447,15 +447,15 @@
             feature_min = nn._feature_min.combine(feature_min, max)
         return feature_min
 
     @property
     def _target_names(self):
         target_names = pd.Series()
         for nn in self._nns:
-            target_names = target_names.append(nn._target_names)
+            target_names = pd.concat([target_names, nn._target_names]).reset_index(drop=True)
         target_names = pd.Series(target_names.unique())
         return target_names
 
     @property
     def _target_max(self):
         target_max = pd.Series(
             np.full_like(self._nns[0]._target_max, np.inf),
```

### Comparing `qlknn-1.2.1/qlknn/models/cython_mkl_ndnn.py` & `qlknn-1.3.1/qlknn/models/cython_mkl_ndnn.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/ffnn.py` & `qlknn-1.3.1/qlknn/models/ffnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*-
 import json
 import os
 from warnings import warn
 from collections import OrderedDict
 
-import numpy as np
+import numpy
 import pandas as pd
 from IPython import embed
+np = numpy
 
 
 def sigm_tf(x):
     return 1.0 / (1 + np.exp(-1 * x))
 
 
 # def sigm(x):
@@ -204,21 +205,26 @@
 
     @property
     def _feature_min(self):
         return self._nn._feature_min
 
 
 class QuaLiKizNDNN:
-    def __init__(self, nn_dict, target_names_mask=None, layer_mode=None, GB_scale_length=1):
+    def __init__(self, nn_dict, target_names_mask=None, layer_mode=None, GB_scale_length=1, np=None):
         """General ND fully-connected multilayer perceptron neural network
 
         Initialize this class using a nn_dict. This dict is usually read
         directly from JSON, and has a specific structure. Generate this JSON
         file using the supplied function in QuaLiKiz-Tensorflow
+
+        np: Override use of standard numpy, route calls through a "duck typed" replacement of numpy.
         """
+        if np is None:
+          np = numpy
+        self.np = np
         parsed = {}
         if layer_mode is None:
             try:
                 import qlknn_intel
             except:
                 layer_mode = "classic"
             else:
@@ -272,15 +278,15 @@
                 if layer_mode == "classic":
                     if activation == "tanh":
                         act = np.tanh
                     elif activation == "relu":
                         act = _act_relu
                     elif activation == "none":
                         act = _act_none
-                    self.layers.append(QuaLiKizNDNN.NNLayer(weight, bias, act))
+                    self.layers.append(QuaLiKizNDNN.NNLayer(weight, bias, act, np))
                 elif layer_mode == "intel":
                     self.layers.append(qlknn_intel.Layer(weight, bias, activation))
                 elif layer_mode == "cython":
                     self.layers.append(cython_mkl_ndnn.Layer(weight, bias, activation))
             except KeyError:
                 # This name does not exist in the JSON,
                 # so our previously read layer was the output layer
@@ -308,15 +314,15 @@
             warn("nn_dict not fully parsed! " + str(parsed))
 
     def apply_layers(self, input, output=None):
         """Apply all NN layers to the given input
 
         The given input has to be array-like, but can be of size 1
         """
-        input = np.ascontiguousarray(input)
+        input = self.np.ascontiguousarray(input)
         # 3x30 network:
         # 14.1 µs ± 913 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
         # 20.9 µs ± 2.43 µs per loop (mean ± std. dev. of 7 runs, 100000 loops each)
         # 19.1 µs ± 240 ns per loop (mean ± std. dev. of 7 runs, 10000 loops each)
         # 2.67 µs ± 29.7 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
 
         for layer in self.layers:
@@ -331,21 +337,22 @@
 
         output = activation(weight * input + bias)
 
         Where weight is generally a matrix; output, input and bias a vector
         and activation a (sigmoid) function.
         """
 
-        def __init__(self, weight, bias, activation):
+        def __init__(self, weight, bias, activation, np):
+            self._np = np
             self._weights = weight
             self._biases = bias
             self._activation = activation
 
         def apply(self, input, output=None):
-            preactivation = np.dot(input, self._weights) + self._biases
+            preactivation = self._np.dot(input, self._weights) + self._biases
             result = self._activation(preactivation)
             return result
 
         def shape(self):
             return self.weight.shape
 
         def __str__(self):
@@ -365,14 +372,17 @@
         """Calculate the output given a specific input
 
         This function accepts inputs in the form of a dict with
         as keys the name of the specific input variable (usually
         at least the feature_names) and as values 1xN same-length
         arrays.
         """
+
+        np = self.np
+
         # 49.1 ns ± 1.53 ns per loop (mean ± std. dev. of 7 runs, 10000000 loops each)
         nn_input, safe, clip_low, clip_high, low_bound, high_bound = determine_settings(
             self, input, safe, clip_low, clip_high, low_bound, high_bound
         )
 
         # nn_input = self._feature_prescale_factors.values[np.newaxis, :] * nn_input + self._feature_prescale_biases.values
         # 14.3 µs ± 1.08 µs per loop (mean ± std. dev. of 7 runs, 100000 loops each)
@@ -608,15 +618,16 @@
                 high_bound
                 if isinstance(high_bound, (int, float))
                 else high_bound.loc[network._target_names].values
             )
     else:
         if input.__class__ == pd.DataFrame:
             nn_input = input.values
-        elif input.__class__ == np.ndarray:
+        else:
+            # numpy ndarray or object behaving like it (e.g. jax array)
             nn_input = input
 
     if clip_low is True and (low_bound is None):
         low_bound = network._target_min.values
     if clip_high is True and (high_bound is None):
         high_bound = network._target_max.values
     return nn_input, safe, clip_low, clip_high, low_bound, high_bound
```

### Comparing `qlknn-1.2.1/qlknn/models/kerasmodel.py` & `qlknn-1.3.1/qlknn/models/kerasmodel.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/qlknn_fortran.py` & `qlknn-1.3.1/qlknn/models/qlknn_fortran.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/qlknn_hyper_10D.py` & `qlknn-1.3.1/qlknn/models/qlknn_hyper_10D.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/qlknnmodule.c` & `qlknn-1.3.1/qlknn/models/qlknnmodule.c`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/rotdiv.py` & `qlknn-1.3.1/qlknn/models/rotdiv.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/setup.py` & `qlknn-1.3.1/qlknn/models/setup.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/models/victor_rule.py` & `qlknn-1.3.1/qlknn/models/victor_rule.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/pipeline/one_off_tasks.py` & `qlknn-1.3.1/qlknn/pipeline/one_off_tasks.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/pipeline/pipeline.py` & `qlknn-1.3.1/qlknn/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/pipeline/simple_scanner.py` & `qlknn-1.3.1/qlknn/pipeline/simple_scanner.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/pipeline/train_NDNN_marconi.sh` & `qlknn-1.3.1/qlknn/pipeline/train_NDNN_marconi.sh`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/pipeline/train_launch.py` & `qlknn-1.3.1/qlknn/pipeline/train_launch.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/HornNet_slice.py` & `qlknn-1.3.1/qlknn/plots/HornNet_slice.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/early_stop.py` & `qlknn-1.3.1/qlknn/plots/comparison/early_stop.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/filter.py` & `qlknn-1.3.1/qlknn/plots/comparison/filter.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/goodness.py` & `qlknn-1.3.1/qlknn/plots/comparison/goodness.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/query_to_networks.py` & `qlknn-1.3.1/qlknn/plots/comparison/query_to_networks.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/regularization.py` & `qlknn-1.3.1/qlknn/plots/comparison/regularization.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/similarity.py` & `qlknn-1.3.1/qlknn/plots/comparison/similarity.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/comparison/topology.py` & `qlknn-1.3.1/qlknn/plots/comparison/topology.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/default_settings_HornNet_slice.json` & `qlknn-1.3.1/qlknn/plots/default_settings_HornNet_slice.json`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/error_heatmap.py` & `qlknn-1.3.1/qlknn/plots/error_heatmap.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/hyperpar_scan.py` & `qlknn-1.3.1/qlknn/plots/hyperpar_scan.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/load_data.py` & `qlknn-1.3.1/qlknn/plots/load_data.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/measures_of_goodness.py` & `qlknn-1.3.1/qlknn/plots/measures_of_goodness.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,124 +22,125 @@
 def deconstruct_varname(varname):
     flux, species, regime, normalization, _ = re.compile(
         "(?=.*)(.)(|ITG|ETG|TEM)_(GB|SI|cm)"
     ).split(varname)
     return flux, species, regime, normalization
 
 
-target_names = ["efeITG_GB", "efiITG_GB", "pfeITG_GB"]
-__, __, regime, norm = deconstruct_varname(target_names[0])
-leading = {"ITG": "efe", "TEM": "efi", "ETG": "efe"}
-leading_flux = leading[regime] + regime + "_" + norm
-leading_idx = target_names.index(leading_flux)
-
-query = (
-    Network.select(
-        Network.id.alias("network_id"),
-        PostprocessSlice,
-        Postprocess.rms,
+if __name__ == "__main__":
+    target_names = ["efeITG_GB", "efiITG_GB", "pfeITG_GB"]
+    __, __, regime, norm = deconstruct_varname(target_names[0])
+    leading = {"ITG": "efe", "TEM": "efi", "ETG": "efe"}
+    leading_flux = leading[regime] + regime + "_" + norm
+    leading_idx = target_names.index(leading_flux)
+
+    query = (
+        Network.select(
+            Network.id.alias("network_id"),
+            PostprocessSlice,
+            Postprocess.rms,
+        )
+        .join(PostprocessSlice, JOIN.LEFT_OUTER)
+        .switch(Network)
+        .join(Postprocess, JOIN.LEFT_OUTER)
+        .switch(Network)
+        .where(Network.target_names == target_names)
+        # .join(PureNetworkParams)
     )
-    .join(PostprocessSlice, JOIN.LEFT_OUTER)
-    .switch(Network)
-    .join(Postprocess, JOIN.LEFT_OUTER)
-    .switch(Network)
-    .where(Network.target_names == target_names)
-    # .join(PureNetworkParams)
-)
-# .join(Hyperparameters,  on=(Network.id == Hyperparameters.network_id))
-# .join(NetworkMetadata,  on=(Network.id == NetworkMetadata.network_id))
-# .join(TrainMetadata,    on=(Network.id == TrainMetadata.network_id))
-# .join(PostprocessSlice, on=(Network.id == PostprocessSlice.network_id))
-# .join(Postprocess, on=(Network.id == Postprocess.network_id))
-# .where(Network.target_names == target_names)
-# .where(TrainMetadata.set == 'train')
-# .where((PostprocessSlice.dual_thresh_mismatch_median == 0) | PostprocessSlice.dual_thresh_mismatch_median.is_null())
-# )
-if query.count() > 0:
-    results = list(query.dicts())
-    df = pd.DataFrame(results)
-    # df['network'] = df['network'].apply(lambda el: 'pure_' + str(el))
-    # df['l2_norm'] = df['l2_norm'].apply(np.nanmean)
-    df.drop(["id", "network"], inplace=True, axis="columns")
-    df.set_index("network_id", inplace=True)
-    stats = df
-else:
-    stats = pd.DataFrame()
-
-for net_id in stats.index:
-    res_dict = {}
-    for param in ["cost_l2_scale", "hidden_neurons"]:
-        res = Network.get_by_id(net_id).flat_recursive_property(param)
-        if isinstance(res, np.ndarray):
-            res = res.astype(object)
-        df.set_value(net_id, param, res)
-
-stats = stats.applymap(np.array)
-# stats[stats.isnull()] = np.NaN
-stats.sort_index(inplace=True)
-stats.dropna(axis="columns", how="all", inplace=True)
-#'no_pop_frac', 'no_thresh_frac', 'pop_abs_mis_95width',
-#       'pop_abs_mis_median', 'rms_test', 'thresh_rel_mis_95width',
-#       'thresh_rel_mis_median', 'l2_norm_weighted'
-# print(stats.max())
-# print(stats.min())
-# print(stats.mean())
-# print(stats.abs().mean())
-dont_care = [
-    "frac",
-    "no_dual_thresh_frac",
-    "no_pop_frac",
-    "no_thresh_frac",
-    "pop_abs_mis_95width",
-    "thresh_rel_mis_95width",
-    "wobble_tot",
-    "wobble_unstab",
-]
-stats.drop(dont_care, axis="columns", inplace=True, errors="ignore")
-array_care = ["pop_abs_mis_median", "thresh_rel_mis_median", "wobble_qlkunstab", "rms"]
-for var in array_care:
-    stats[var] = stats.agg({var: lambda x: x[leading_idx]})
-embed()
-
-stats["rms"] = stats.pop("rms")
-stats["thresh"] = stats.pop("thresh_rel_mis_median").abs().apply(np.max)
-stats["no_thresh_frac"] = stats.pop("no_thresh_frac").apply(np.max)
-stats["pop"] = (14 - stats.pop("pop_abs_mis_median").abs()).apply(np.max)
-if "wobble_tot" in stats.keys():
-    stats["wobble_tot"] = stats.pop("wobble_tot").apply(np.max)
-    stats["wobble_unstab"] = stats.pop("wobble_unstab").apply(np.max)
-stats["pop_frac"] = (1 - stats.pop("no_pop_frac")).apply(np.max)
-# stats.dropna(inplace=True)
-try:
-    del stats["dual_thresh_mismatch_95width"]
-    stats["thresh_mismatch"] = stats.pop("dual_thresh_mismatch_median").abs().apply(np.max)
-except KeyError:
-    pass
-# (stats/stats.max()).nsmallest(10, 'rms').plot.bar()
-
-fig = plt.figure()
-gs = gridspec.GridSpec(
-    2,
-    1,
-    height_ratios=[10, 2],
-    width_ratios=[1],
-    left=0.05,
-    right=0.95,
-    wspace=0.05,
-    hspace=0.05,
-)
-ax2 = plt.subplot(gs[1, 0])
-ax1 = plt.subplot(gs[0, 0])
-top = (stats).nsmallest(10, "rms")
-top.dropna("columns", inplace=True)
-subplot = (top / top.max()).plot.bar(ax=ax1)
-text = [(col, "{:.2f}".format(top[col].max())) for col in top]
-text = list(map(list, zip(*text)))  # Transpose
-table = ax2.table(cellText=text, cellLoc="center")
-table.auto_set_font_size(False)
-table.scale(1, 1.5)
-# table.set_fontsize(20)
-ax2.axis("tight")
-ax2.axis("off")
-# (np.log10(stats/stats.max())).loc[stats.sum(axis='columns').nsmallest(10).index].plot.bar()
-# plt.show()
-embed()
+    # .join(Hyperparameters,  on=(Network.id == Hyperparameters.network_id))
+    # .join(NetworkMetadata,  on=(Network.id == NetworkMetadata.network_id))
+    # .join(TrainMetadata,    on=(Network.id == TrainMetadata.network_id))
+    # .join(PostprocessSlice, on=(Network.id == PostprocessSlice.network_id))
+    # .join(Postprocess, on=(Network.id == Postprocess.network_id))
+    # .where(Network.target_names == target_names)
+    # .where(TrainMetadata.set == 'train')
+    # .where((PostprocessSlice.dual_thresh_mismatch_median == 0) | PostprocessSlice.dual_thresh_mismatch_median.is_null())
+    # )
+    if query.count() > 0:
+        results = list(query.dicts())
+        df = pd.DataFrame(results)
+        # df['network'] = df['network'].apply(lambda el: 'pure_' + str(el))
+        # df['l2_norm'] = df['l2_norm'].apply(np.nanmean)
+        df.drop(["id", "network"], inplace=True, axis="columns")
+        df.set_index("network_id", inplace=True)
+        stats = df
+    else:
+        stats = pd.DataFrame()
+
+    for net_id in stats.index:
+        res_dict = {}
+        for param in ["cost_l2_scale", "hidden_neurons"]:
+            res = Network.get_by_id(net_id).flat_recursive_property(param)
+            if isinstance(res, np.ndarray):
+                res = res.astype(object)
+            df.set_value(net_id, param, res)
+
+    stats = stats.applymap(np.array)
+    # stats[stats.isnull()] = np.NaN
+    stats.sort_index(inplace=True)
+    stats.dropna(axis="columns", how="all", inplace=True)
+    #'no_pop_frac', 'no_thresh_frac', 'pop_abs_mis_95width',
+    #       'pop_abs_mis_median', 'rms_test', 'thresh_rel_mis_95width',
+    #       'thresh_rel_mis_median', 'l2_norm_weighted'
+    # print(stats.max())
+    # print(stats.min())
+    # print(stats.mean())
+    # print(stats.abs().mean())
+    dont_care = [
+        "frac",
+        "no_dual_thresh_frac",
+        "no_pop_frac",
+        "no_thresh_frac",
+        "pop_abs_mis_95width",
+        "thresh_rel_mis_95width",
+        "wobble_tot",
+        "wobble_unstab",
+    ]
+    stats.drop(dont_care, axis="columns", inplace=True, errors="ignore")
+    array_care = ["pop_abs_mis_median", "thresh_rel_mis_median", "wobble_qlkunstab", "rms"]
+    for var in array_care:
+        stats[var] = stats.agg({var: lambda x: x[leading_idx]})
+    embed()
+
+    stats["rms"] = stats.pop("rms")
+    stats["thresh"] = stats.pop("thresh_rel_mis_median").abs().apply(np.max)
+    stats["no_thresh_frac"] = stats.pop("no_thresh_frac").apply(np.max)
+    stats["pop"] = (14 - stats.pop("pop_abs_mis_median").abs()).apply(np.max)
+    if "wobble_tot" in stats.keys():
+        stats["wobble_tot"] = stats.pop("wobble_tot").apply(np.max)
+        stats["wobble_unstab"] = stats.pop("wobble_unstab").apply(np.max)
+    stats["pop_frac"] = (1 - stats.pop("no_pop_frac")).apply(np.max)
+    # stats.dropna(inplace=True)
+    try:
+        del stats["dual_thresh_mismatch_95width"]
+        stats["thresh_mismatch"] = stats.pop("dual_thresh_mismatch_median").abs().apply(np.max)
+    except KeyError:
+        pass
+    # (stats/stats.max()).nsmallest(10, 'rms').plot.bar()
+
+    fig = plt.figure()
+    gs = gridspec.GridSpec(
+        2,
+        1,
+        height_ratios=[10, 2],
+        width_ratios=[1],
+        left=0.05,
+        right=0.95,
+        wspace=0.05,
+        hspace=0.05,
+    )
+    ax2 = plt.subplot(gs[1, 0])
+    ax1 = plt.subplot(gs[0, 0])
+    top = (stats).nsmallest(10, "rms")
+    top.dropna("columns", inplace=True)
+    subplot = (top / top.max()).plot.bar(ax=ax1)
+    text = [(col, "{:.2f}".format(top[col].max())) for col in top]
+    text = list(map(list, zip(*text)))  # Transpose
+    table = ax2.table(cellText=text, cellLoc="center")
+    table.auto_set_font_size(False)
+    table.scale(1, 1.5)
+    # table.set_fontsize(20)
+    ax2.axis("tight")
+    ax2.axis("off")
+    # (np.log10(stats/stats.max())).loc[stats.sum(axis='columns').nsmallest(10).index].plot.bar()
+    # plt.show()
+    embed()
```

### Comparing `qlknn-1.2.1/qlknn/plots/plot_camille_NNs.py` & `qlknn-1.3.1/qlknn/plots/plot_camille_NNs.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/plot_nn_structure.py` & `qlknn-1.3.1/qlknn/plots/plot_nn_structure.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/popplots.py` & `qlknn-1.3.1/qlknn/plots/popplots.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/qlk_slice_plot_camille.py` & `qlknn-1.3.1/qlknn/plots/qlk_slice_plot_camille.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/quickslicer.py` & `qlknn-1.3.1/qlknn/plots/quickslicer.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,19 +57,15 @@
         )
         from qlknn.NNDB.model import *
 
         have_nndb_functionality = True
     except:
         logger.warning("No NNDB access")
 
-global nns, slicedim, df, style, col_names_loc, col_names  # Yes I use globals, deal with it
-nns = None
-slicedim = None
-df = None
-style = None
+global col_names_loc, col_names  # Yes I use globals, deal with it
 col_names_loc = None
 col_names = None
 
 
 def mode_to_settings(mode):
     settings = {}
     if mode == "debug":
@@ -441,15 +437,15 @@
     logger.info("Converting to float64")
     df = df.astype("float64")
     logger.info("dataset loaded!")
     return df
 
 
 def check_if_same_order(df, nns, slicedim):
-    """ Check if feature_names of the nns match the df column order"""
+    """Check if feature_names of the nns match the df column order"""
     is_same_order = True
     for nn in nns.values():
         slicedim_idx = nn._feature_names[nn._feature_names == slicedim].index[0]
         varlist = list(df.index.names)
         varlist.insert(slicedim_idx, slicedim)
         try:
             if ~np.all(varlist == nn._feature_names):
@@ -547,34 +543,37 @@
             logger.debug("No threshold3")
 
     return thresh
 
 
 # 5.4 ms ± 115 µs per loop (mean ± std. dev. of 7 runs, 100 loops each) total
 def process_chunk(
-    target_names, chunck, thresh_method="2", settings=None, safe=True, column_map=None
+    target_names, chunk, nns, thresh_method="2", settings=None, safe=True, column_map=None
 ):
-
     res = []
-    for ii, row in enumerate(chunck.iterrows()):
+    for ii, row in enumerate(chunk.iterrows()):
+        # Hacky way to inject some more information to calling functions
+        row[1].index.names = ["dataset", row[1].index.names[1]]
         res.append(
             process_row(
                 target_names,
+                list(chunk.index.names),
                 row,
+                nns,
                 thresh_method=thresh_method,
                 settings=settings,
                 safe=safe,
                 column_map=column_map,
             )
         )
     return res
 
 
 def map_column_name_to_index_map(df, nns):
-    """ Generate a map from QLKNN output names to numpy matrix indices"""
+    """Generate a map from QLKNN output names to numpy matrix indices"""
     column_map = []
     col_names = []
     if nns is not None:
         max_target_length = max(len(nn._target_names) for nn in nns.values())
         column = 0
         for ii, nn in enumerate(nns.values()):
             target_names = nn._target_names.to_list()
@@ -595,15 +594,17 @@
         if len(column_map) != len(col_names):
             raise RuntimeError("Column names different length than produced map")
     return column_map, col_names
 
 
 def process_row(
     target_names,
+    feature_names,
     row,
+    nns,
     thresh_method="2",
     ax1=None,
     safe=True,
     settings=None,
     column_map=None,
 ):
     """Process a single 'row' or 'slice'
@@ -633,16 +634,19 @@
         )
     if nns is not None and column_map is None:
         raise Exception("Provide a map from NN names to columns, or the rest will fail")
     if column_map is not None:
         column_map_clean = [el for el in column_map if el >= 0]
     index, slice_ = row
     feature = slice_.index.levels[1]
-    target = slice_.values[: len(feature) * len(target_names)].reshape(
-        len(target_names), len(feature)
+    datasets = slice_.index.levels[0]
+    # We "fold" our numpy array such that it is 2D with dimensions
+    # nout * ndatasets, nin
+    target = slice_.values[: len(feature) * len(target_names) * len(datasets)].reshape(
+        len(target_names) * len(datasets), len(feature)
     )
 
     target_idx = slice_.index.get_level_values(0)
     target_rownames = target_idx[target_idx.duplicated()].unique()
     logger.debug("Current slice:\n {!s}".format(slice_))
     logger.debug("Numpy style slice:\n {!s}".format(target))
     logger.debug("With rows: {!s}".format(target_rownames))
@@ -669,14 +673,15 @@
         if settings["plot_zerocolors"]:
             maxgam = slice_["maxgam"]
 
         # Create slice, assume sorted
         # 14.8 µs ± 1.27 µs per loop (mean ± std. dev. of 7 runs, 100000 loops each)
         x = np.linspace(feature.values[0], feature.values[-1], 200)
         # if plot:
+        slicedim = slice_.axes[0].names[-1]
         if not ax1 and settings["plot"]:
             fig = plt.figure()
             if settings["plot_pop"] and settings["plot_slice"]:
                 gs = gridspec.GridSpec(
                     2,
                     2,
                     height_ratios=[10, 1],
@@ -801,17 +806,18 @@
                 slice_dict = {
                     name: np.full_like(x, val) for name, val in zip(df.index.names, index)
                 }
                 slice_dict[slicedim] = x
 
         # Plot target points
         if settings["plot"] and settings["plot_slice"]:
+            assert len(index) == len(feature_names)
             table = ax2.table(
                 cellText=[
-                    [nameconvert[name] for name in df.index.names],
+                    [nameconvert[name] for name in feature_names],
                     ["{:.2f}".format(xx) for xx in index],
                 ],
                 cellLoc="center",
             )
             table.auto_set_font_size(False)
             table.scale(1, 1.5)
             # table.set_fontsize(20)
@@ -968,15 +974,15 @@
                 popback[popback == x[-1]] = np.nan
             else:
                 for ii, row in enumerate(nn_preds.T):
                     if not np.isnan(thresh_nn[ii]):
                         try:
                             popback_i = np.flatnonzero(row[: thresh_nn_i[ii]])
                             popbacks[ii] = x[popback_i[-1]]
-                        except (IndexError):
+                        except IndexError:
                             popbacks[ii] = np.nan
                     else:
                         popbacks[ii] = np.nan
 
             # 5.16 µs ± 188 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
 
             # Calculate wobbles of evaulated nets
@@ -984,15 +990,14 @@
             wobble_tot_loc = np.mean(wobble_loc, axis=0)
             with warnings.catch_warnings():  # col[ind:] is empty if no threshold
                 warnings.simplefilter("ignore", category=RuntimeWarning)
                 wobble_unstab_loc = np.array(
                     [np.mean(col[ind:]) for ind, col in zip(thresh_nn_i + 1, wobble_loc.T)]
                 )
             try:
-
                 with warnings.catch_warnings():  # col[ind:] is empty if no threshold
                     warnings.simplefilter("ignore", category=RuntimeWarning)
                     thresh_2_i = np.where(np.abs(x - thresh) == np.min(np.abs(x - thresh)))[0][0]
                 with warnings.catch_warnings():  # col[thresh_2_i:] is empty if no threshold
                     warnings.simplefilter("ignore", category=RuntimeWarning)
                     wobble_qlkunstab_loc = np.array(
                         [np.mean(col[thresh_2_i:]) for col in wobble_loc.T]
@@ -1109,23 +1114,23 @@
                 )
             )
         if settings["plot"]:
             ax1.legend()
             ax1.set_ylim(bottom=min(ax1.get_ylim()[0], 0))
             plt.show()
             fig.savefig("slice.pdf", format="pdf", bbox_inches="tight")
-            qlk_data = pd.DataFrame(target.T, columns=target_names, index=feature)
+            qlk_data = pd.DataFrame(target.T, columns=product(target_names, datasets), index=feature)
             if nns is not None:
                 nn_data = pd.DataFrame(nn_preds, columns=col_names_loc)
                 nn_data.index = x
                 nn_data.index.name = feature.name
-                slice_data = pd.Series(dict(zip(df.index.names, index)))
+                slice_data = pd.Series(dict(zip(feature_names, index)))
                 slice_latex = (
-                    ("  {!s} &" * len(df.index.names))
-                    .format(*[nameconvert[name] for name in df.index.names])
+                    ("  {!s} &" * len(feature_names))
+                    .format(*[nameconvert[name] for name in feature_names])
                     .strip(" &")
                 )
                 slice_latex += ("\\\\\n" + " {:.2f} &" * len(index)).format(*index).strip(" &")
             # embed()
             plt.close(fig)
         if not isinstance(thresh, float):
             logger.warning("Threshold not a float, should look at this..")
@@ -1211,14 +1216,15 @@
     else:
         duo_results = pd.DataFrame()
     return results, duo_results
 
 
 def extract_nn_stats(results, duo_results, nns, frac, store_name, submit_to_nndb=False):
     try:
+        logger.info("Connecting to NNDB")
         db.connect()
     except (OperationalError, NameError):
         logger.warning("No access to NNDB, aborting NNDB connection!")
         return
     for network_name, res in results.unstack().iterrows():
         network_class, network_number = network_name.split("_")
         nn = nns[network_name]
@@ -1265,21 +1271,23 @@
 def initialize_argument_parser(parser: ArgumentParser) -> ArgumentParser:
     parser.description = """
 Slice  QLKNN datasets and collect stats of QLKNN-style
 Neural Networks (NNs). These networks can be stored locally in a
 file, or in the Neural Network DataBase (NNDB)
 """
     parser.add_argument(
-        "dataset_path", type=Path, help="Path to the to-be sliced pandas HDF5 file"
+        "dataset_paths",
+        type=Path,
+        help="Path to the to-be sliced pandas HDF5 file",
+        nargs="*",
     )
 
     parser.add_argument(
-        "nn_source",
+        "--nn-source",
         type=Path,
-        nargs="?",
         help="Source where the NNs will be pulled from. Can be a path to a file,"
         " or the special key 'NNDB' to pull unsliced networks from the NNDB",
     )
 
     # Add "general arguments"
     parser.add_argument("--verbosity", "-v", default=0, action="count")
     parser.add_argument("--quiet", "-q", action="store_true")
@@ -1367,22 +1375,23 @@
     )
     parser.add_argument(
         "--dump-slice-output",
         action="store_true",
         help="Dump a HDF5 with the sliced outputs to disk",
     )
     parser.add_argument("--no-shuffle", action="store_true", help="Do not shuffle data")
+    parser.add_argument("--connect-nndb", action="store_true", help="Connect to the NNDB")
     parser.set_defaults(func=main)
     return parser
 
 
 def main(namespace: Optional[Namespace] = None):
-    """ Main Quickslicer CLI entry point """
+    """Main Quickslicer CLI entry point"""
     # multiprocess parallelism uses globals to share state. Probably can be done safer, but this is simple and fast
-    global slicedim, df, style, col_names_loc, col_names, nns  # Yes I use globals, deal with it
+    global col_names_loc, col_names  # Yes I use globals, deal with it
 
     if not namespace:
         parser = argparse.ArgumentParser()
         parser: ArgumentParser = initialize_argument_parser(parser)
         args: Namespace = parser.parse_args()
     else:
         args = namespace
@@ -1430,18 +1439,25 @@
 
     dump_slice_input_to_disk = args.dump_slice_input
     dump_slice_output_to_disk = args.dump_slice_output
 
     shuffle = not args.no_shuffle
 
     # Find on-disk dataset
-    store = pd.HDFStore(args.dataset_path, "r")
-    if len(store.groups()) < 1:
-        raise TypeError(f"{args.dataset_path} is empty, are you sure this is a pd.HDFStore?")
-    store_basename = args.dataset_path.name
+    dataset_path = args.dataset_paths[0]
+    stores = {}
+    for ii, dataset_path in enumerate(args.dataset_paths):
+        store = pd.HDFStore(dataset_path, "r")
+        if len(store.groups()) < 1:
+            raise TypeError(f"{dataset_path} is empty, are you sure this is a pd.HDFStore?")
+        store_basename = dataset_path.name
+        stores[store_basename] = store
+        if ii == 0:
+            ref_store_name = store_basename
+        del store, store_basename
 
     # Load to-be-sliced NNs
     if nn_source == "NNDB":
         try:
             __, dim, __ = get_store_params(store_basename)
         except:
             logger.critical(
@@ -1474,22 +1490,24 @@
         nn_source_module = importlib.import_module(module_name)
         nns = nn_source_module.nns
         if slicedim is None:
             slicedim = nn_source_module.slicedim
         style = nn_source_module.style
         sys.path.remove(module_folder)
 
+    # Try to auto-detect our feature_names and target_names.
+    # If we have NNs this is easy!
     if nns is not None:
         nn0 = list(nns.values())[0]
         feature_names = nn0._feature_names
         if target_names is None:
             target_names = nn0._target_names
     else:
         feature_names = pd.Series(
-            name.decode("UTF-8") for name in store.get_node("input").axis0.read()
+            name.decode("UTF-8") for name in stores[ref_store_name].get_node("input").axis0.read()
         )
         if target_names is None:
             raise Exception("Please pass --slice-targets when slicing without NNs")
         if slicedim is None:
             driving_gradient_list = determine_driving_gradients("_dummy_".join(target_names))
             if len(driving_gradient_list) >= 1:
                 driving_gradient = driving_gradient_list[0]  # Just take the first gradient
@@ -1530,33 +1548,53 @@
         filter_geq = None
         filter_less = None
     else:
         clip = True
         filter_geq = -120
         filter_less = 120
 
-    # Prepare the dataset: fold into slices and re-order in NN order if necessary
-    # Returns the folded dataset
-    df = prep_df(
-        store,
+    # Prepare the dataset: fold into slices and re-order in NN order if
+    # necessary. Returns the folded dataset. Note that this puts values
+    # to NaN! We first slice our "reference" DataFrame
+    df_ref = prep_df(
+        stores.pop(ref_store_name),
         feature_names,
         target_names,
         slicedim,
         filter_less=filter_less,
         filter_geq=filter_geq,
         myslice=myslice,
         frac=frac,
         GB_scale=GB_scale,
         shuffle=shuffle,
     )
-    gc.collect()
+    dfs = {ref_store_name: df_ref}
+    # Now it becomes tricky, as we need to find the same slice as in our
+    # reference in the _other_datasets
+    for store_basename, store in stores.items():
+        logger.info("Preparing dataset %s", store_basename)
+        # Do not pass frac nor shuffle, as that will result in this
+        # DataFrame being misaligned with our reference Frame
+        df = prep_df(
+            store,
+            feature_names,
+            target_names,
+            slicedim,
+            filter_less=filter_less,
+            filter_geq=filter_geq,
+            myslice=myslice,
+            GB_scale=GB_scale,
+        )
+        dfs[store_basename] = df.loc[df_ref.index]
+        del df
+        gc.collect()
     # Check if the dataset is indeed in the same order as _all_ the nns feature names.
     # If not, will need some special handling
     if nns is not None:
-        is_same_order = check_if_same_order(df, nns, slicedim)
+        is_same_order = check_if_same_order(df_ref, nns, slicedim)
     else:
         is_same_order = True
     if not is_same_order:
         logger.warning(
             "Networks and dataset have features in a different order! Forcing safe mode!"
         )
         safe = True
@@ -1587,24 +1625,74 @@
         mpl.rcParams.update({"font.size": 16})
     else:
         if hasattr(target_names, "index") and hasattr(target_names.index, "names"):
             target_names_list = target_names.index.names
         else:
             target_names_list = list(target_names)
         nameconvert = {
-            name: name for name in df.columns.names + df.index.names + target_names_list
+            name: name
+            for name in dfs[ref_store_name].columns.names
+            + dfs[ref_store_name].index.names
+            + target_names_list
         }
 
     # Thresholds only calculated on first target name
     if len(target_names) > 1 and len(thresh_methods) != 0:
         logger.warning("Thresholds are only calculated on the first target name")
 
-    column_map, col_names = map_column_name_to_index_map(df, nns)
+    column_map, col_names = map_column_name_to_index_map(dfs[ref_store_name], nns)
     col_names_loc = col_names
 
+    # Now let us make a MEGA frame
+    if len(dfs) > 1:
+        logger.info("Combining all datasets into a MEGA dataset")
+        logger.warning("This is an experimental feature!")
+        # Take one dataset as reference/main dataset.
+        main_df: pd.DataFrame = dfs.pop(ref_store_name)
+        # main_df = pd.concat([main_df], keys=[ref_store_name], names=['dataset'])
+        # And start looping over the rest of the datasets
+        for ii, (store_name, df) in enumerate(dfs.items()):
+            # We have _guaranteed_ duplicate column names, as this is how we
+            # prepared the datasets. So, to be efficient we need to merge in
+            # Two steps. First on Index:
+            # df = pd.concat([df], keys=[store_name], names=['dataset'])
+            main_df = main_df.join(
+                df, how="outer", rsuffix=f"-{ii+1}", lsuffix=f"-{ii}", sort=True
+            )
+            # Now we have a huge df with "duplicate" columns, something like:
+            # main_df.columns = pd. MultiIndex([('efeETG_GB-0',   5.0),
+            #                                   ('efeETG_GB-0',  10.0),
+            #                                   ('efeETG_GB-0',  15.0),
+            #                                   ('efeETG_GB-0', 140.0),
+            #                                   ('efeETG_GB-0', 150.0),
+            #                                   ('efeETG_GB-1',   5.0),
+            #                                   ('efeETG_GB-1', 140.0),
+            #                                   ('efeETG_GB-1', 150.0)],
+            #                                   names=[None, 'Ate'])
+            # Which we might need to merge in an inefficient step. Lets hope at
+            # least  the spatial grid is similar or at the very least small.
+            # I'm assuming that for now, and keeping this piece of code to
+            # merge it for now
+            # xgrid = np.unique(main_df.columns.get_level_values(slicedim))
+            # data = {}
+            # datum_remapper = {f"{xx}-{yy}": yy for xx, yy in product(target_names_list, range(len(dfs)+1))}
+            # for xpoint in xgrid:
+            #    datum = main_df.loc[:, (slice(None), xpoint)]
+            #    datum = datum.stack(0)
+            #    datum.rename(datum_remapper, inplace=True)
+            #    datum.index.names = list(datum.index.names[:-1]) + ["dataset"]
+            #    data[xpoint] = datum
+            # main_df = pd.concat(data)
+            # del data, datum, xgrid, datum_remapper
+            # gc.collect()
+    else:
+        main_df = dfs[ref_store_name]
+    del dfs
+    gc.collect()
+
     # Try to determine if we want to run in parallel. Plotting in parallel is not a good idea
     # so 'debug' mode and 'pretty' mode try to run serially. quick mode tries to be parallel
     running_parallel = (settings["parallel"] and parallel_forced is None) or (
         parallel_forced is True
     )
     if running_parallel:
         num_processes = cpu_count()
@@ -1615,50 +1703,55 @@
         chunks = [df.loc[df.index[i : i + chunk_size]] for i in range(0, df.shape[0], chunk_size)]
         pool = Pool(processes=num_processes)
         logger.info("Using {:d} processes".format(num_processes))
     else:
         logger.info("Running in serial mode")
 
     if nns is not None:
-        logger.info("Starting {:d} slices for {:d} networks".format(len(df), len(nns)))
+        logger.info("Starting {:d} slices for {:d} networks".format(len(main_df), len(nns)))
     else:
-        logger.info("Starting {:d} slices without networks".format(len(df)))
+        logger.info("Starting {:d} slices without networks".format(len(main_df)))
     starttime = time.time()
 
     if not running_parallel:
         results = [
-            process_chunk(target_names, df, settings=settings, safe=safe, column_map=column_map)
+            process_chunk(
+                target_names, main_df, nns, settings=settings, safe=safe, column_map=column_map
+            )
         ]
     else:
         results = pool.map(
             partial(
                 process_chunk,
                 target_names,
                 settings=settings,
                 safe=safe,
                 column_map=column_map,
             ),
             chunks,
         )
 
-    logger.info("{!s} took {!s} seconds".format(len(df), time.time() - starttime))
+    logger.info(
+        "{!s} took {!s} seconds, collecting results".format(len(main_df), time.time() - starttime)
+    )
 
     zero_slices = 0
     totstats = []
     qlk_thresh = []
     index = []
     # This loops over each _row_
     for islice, result in enumerate(chain(*results)):
         if result[0] == 1:
             zero_slices += 1
         else:
             totstats.append(result[2])
             qlk_thresh.append(result[1])
             index.append(islice)
 
+    logger.info("Results collected, consolidating")
     stats = ["thresh", "pop", "wobble_tot", "wobble_unstab", "wobble_qlkunstab"]
     if nns is None:
         totstats = pd.DataFrame(
             totstats,
             index=index,
             columns=pd.MultiIndex.from_tuples(list(product(["dummy"], stats))),
         )
@@ -1677,43 +1770,53 @@
     qlk_data = pd.DataFrame(
         qlk_data, index=index, columns=pd.MultiIndex.from_product([qlk_columns, stats])
     )
     qlk_data.columns.names = ("line", "stat")
 
     totstats = totstats.join(qlk_data)
 
+    logger.info("Results consolidated, generating reports")
     totstats_filename = runname + "_totstats.h5.1"
     if dump_totstats_to_disk:
+        logger.info("Dumping totstats to disk as requested, this might take a while")
         print('Writing totstats to "{!s}"'.format(totstats_filename))
         totstats.to_hdf(totstats_filename, "stats", format="table", complevel=1)
 
+    logger.info("Extracting dataset stats")
     res, duo_res = extract_stats(totstats, style)
     res.index.names = ["network_label", "target_names"]
     if len(duo_res) != 0:
         duo_res.index.names = ["network_label", "target_names"]
 
     # dump to disk
     if dump_to_disk:
-        dump_results_to_disk(res, duo_res, frac, store_basename, runname=runname)
+        logger.info("Dumping results to disk as requested, this might take a while")
+        dump_results_to_disk(res, duo_res, frac, ref_store_name, runname=runname)
 
-    if nns is not None:
+    if args.connect_nndb:
         try:
+            logger.info("Extracting Neural Network stats")
             extract_nn_stats(
-                res, duo_res, nns, frac, store_basename, submit_to_nndb=submit_to_nndb
+                res, duo_res, nns, frac, ref_store_name, submit_to_nndb=submit_to_nndb
             )
+            logger.info("Extracting Neural Network stats done")
         except:
             logger.warning("Could not extract NNDB stats")
 
     if dump_slice_input_to_disk:
+        logger.info("Dumping slice input to disk as requested, this might take a while")
         print('Writing slice inputs to "{!s}"'.format(totstats_filename))
         inp = df.index.to_frame(index=False)
         inp.to_hdf(totstats_filename, "input", format="table", complevel=1)
 
     if dump_slice_output_to_disk:
+        logger.info("Dumping slice output to disk as requested, this might take a while")
         # This will be numbered per slice, e.g. index 0 for 0th slice
         outp = df.reset_index(drop=True)
         outp = outp.stack().reset_index(-1)
         outp.to_hdf(totstats_filename, "output", format="table", complevel=1)
 
+    logger.info("Main quickslicer script finished")
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `qlknn-1.2.1/qlknn/plots/quickslicer_dummy_net.py` & `qlknn-1.3.1/qlknn/plots/quickslicer_dummy_net.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/plots/statistical_spread.py` & `qlknn-1.3.1/qlknn/plots/statistical_spread.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/setup_logging.py` & `qlknn-1.3.1/qlknn/setup_logging.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/datasets.py` & `qlknn-1.3.1/qlknn/training/datasets.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/default_settings.json` & `qlknn-1.3.1/qlknn/training/default_settings.json`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/edgerun8_settings.json` & `qlknn-1.3.1/qlknn/training/edgerun8_settings.json`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/gridSearch.py` & `qlknn-1.3.1/qlknn/training/gridSearch.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/gridSearch_structure.py` & `qlknn-1.3.1/qlknn/training/gridSearch_structure.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/keras_helpers.py` & `qlknn-1.3.1/qlknn/training/keras_helpers.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/keras_models.py` & `qlknn-1.3.1/qlknn/training/keras_models.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/nn_primitives.py` & `qlknn-1.3.1/qlknn/training/nn_primitives.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/profiling.py` & `qlknn-1.3.1/qlknn/training/profiling.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/train_NDNN.py` & `qlknn-1.3.1/qlknn/training/train_NDNN.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/train_NDNN_cli.py` & `qlknn-1.3.1/qlknn/training/train_NDNN_cli.py`

 * *Files identical despite different names*

### Comparing `qlknn-1.2.1/qlknn/training/train_NDNN_legacy.py` & `qlknn-1.3.1/qlknn/training/train_NDNN_legacy.py`

 * *Files identical despite different names*

