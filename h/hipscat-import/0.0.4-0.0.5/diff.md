# Comparing `tmp/hipscat-import-0.0.4.tar.gz` & `tmp/hipscat-import-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-import-0.0.4.tar", last modified: Tue Jul 11 19:29:51 2023, max compression
+gzip compressed data, was "hipscat-import-0.0.5.tar", last modified: Thu Jul 13 13:38:28 2023, max compression
```

## Comparing `hipscat-import-0.0.4.tar` & `hipscat-import-0.0.5.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/type-checking.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/debug.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/docs/catalogs/public/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/tic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/zubercal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/resume.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/association.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/contact.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/index_table.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/margin_cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/notebooks/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     9556 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/notebooks/estimate_pixel_threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)   136863 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/allwise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/association/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/run_association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/resume_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/run_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/association/
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/association/test_association_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/association/test_association_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/association/test_run_association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_resume_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/resume/intermediate/reducing_log.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (123)  1688789 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.785901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.785901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.785901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)   133704 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.789901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    86295 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    92667 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    99907 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    42210 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    54775 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    72993 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    80298 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (123)   162097 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    43738 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.789901 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/catalog.starr
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/multiindex.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/pandasindex.parquet
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/small_sky.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.789901 hipscat-import-0.0.4/tests/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/index/test_index_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/index/test_index_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/index/test_run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/test_runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/type-checking.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/debug.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/resume.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/association.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/notebooks/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9556 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   136863 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/hipscat_import/association/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/run_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/run_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/association/
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/association/test_association_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/association/test_association_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/association/test_run_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/resume/intermediate/reducing_log.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (123)  1688789 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)   133704 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    86295 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    92667 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    99907 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    42210 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    54775 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    72993 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    80298 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   162097 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    43738 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/multiindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/test_runtime_arguments.py
```

### Comparing `hipscat-import-0.0.4/.github/pull_request_template.md` & `hipscat-import-0.0.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.github/workflows/build-documentation.yml` & `hipscat-import-0.0.5/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.github/workflows/linting.yml` & `hipscat-import-0.0.5/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.github/workflows/publish-to-pypi.yml` & `hipscat-import-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.github/workflows/smoke-test.yml` & `hipscat-import-0.0.5/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.github/workflows/testing-and-coverage.yml` & `hipscat-import-0.0.5/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.github/workflows/type-checking.yml` & `hipscat-import-0.0.5/.github/workflows/type-checking.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.gitignore` & `hipscat-import-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/.pre-commit-config.yaml` & `hipscat-import-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/LICENSE` & `hipscat-import-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/PKG-INFO` & `hipscat-import-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.0.4
+Version: 0.0.5
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-import-0.0.4/README.md` & `hipscat-import-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/Makefile` & `hipscat-import-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/advanced.rst` & `hipscat-import-0.0.5/docs/catalogs/advanced.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/public/allwise.rst` & `hipscat-import-0.0.5/docs/catalogs/public/allwise.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/public/index.rst` & `hipscat-import-0.0.5/docs/catalogs/public/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/public/neowise.rst` & `hipscat-import-0.0.5/docs/catalogs/public/neowise.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/public/tic.rst` & `hipscat-import-0.0.5/docs/catalogs/public/tic.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/public/zubercal.rst` & `hipscat-import-0.0.5/docs/catalogs/public/zubercal.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/catalogs/resume.rst` & `hipscat-import-0.0.5/docs/catalogs/resume.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/conf.py` & `hipscat-import-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/guide/contributing.rst` & `hipscat-import-0.0.5/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/index.rst` & `hipscat-import-0.0.5/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 ========================================================================================
 
 Utility for ingesting large survey data into HiPSCat structure.
 
 Installation
 -------------------------------------------------------------------------------
 
+We recommend installing in a virtual environment, like venv or conda. You may
+need to install or upgrade versions of dependencies to work with hipscat-import.
+
 .. code-block:: bash
 
     pip install hipscat-import
 
 .. tip::
     Installing on Mac
```

### Comparing `hipscat-import-0.0.4/docs/notebooks/estimate_pixel_threshold.ipynb` & `hipscat-import-0.0.5/docs/notebooks/estimate_pixel_threshold.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/static/allwise_schema.parquet` & `hipscat-import-0.0.5/docs/static/allwise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/static/allwise_types.csv` & `hipscat-import-0.0.5/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/static/neowise_types.csv` & `hipscat-import-0.0.5/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/docs/static/tic_types.csv` & `hipscat-import-0.0.5/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/pyproject.toml` & `hipscat-import-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/.pylintrc` & `hipscat-import-0.0.5/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/association/arguments.py` & `hipscat-import-0.0.5/src/hipscat_import/association/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/association/map_reduce.py` & `hipscat-import-0.0.5/src/hipscat_import/association/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/association/run_association.py` & `hipscat-import-0.0.5/src/hipscat_import/association/run_association.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/catalog/arguments.py` & `hipscat-import-0.0.5/src/hipscat_import/catalog/arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Utility to hold all arguments required throughout partitioning"""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Callable, List
+from typing import List
 
-import pandas as pd
 from hipscat.catalog.catalog import CatalogInfo
 from hipscat.io import FilePointer, file_io
 from hipscat.pixel_math import hipscat_id
 
 from hipscat_import.catalog.file_readers import InputReader, get_file_reader
+from hipscat_import.catalog.resume_plan import ResumePlan
 from hipscat_import.runtime_arguments import RuntimeArguments
 
 # pylint: disable=too-many-locals,too-many-arguments,too-many-instance-attributes,too-many-branches,too-few-public-methods
 
 
 @dataclass
 class ImportArguments(RuntimeArguments):
@@ -64,24 +64,21 @@
     mapping_healpix_order: int = -1
     """healpix order to use when mapping. will be
     ``highest_healpix_order`` unless a positive value is provided for
     ``constant_healpix_order``"""
     debug_stats_only: bool = False
     """do not perform a map reduce and don't create a new
     catalog. generate the partition info"""
-    filter_function: Callable | None = None
-    """optional method which takes a pandas dataframe as input, performs some 
-    filtering or transformation of the data, and returns a dataframe with the 
-    rows that will be used to create the new catalog"""
     file_reader: InputReader | None = None
     """instance of input reader that specifies arguments necessary for reading
     from your input files"""
+    resume_plan: ResumePlan | None = None
+    """container that handles read/write of log files for this pipeline"""
 
     def __post_init__(self):
-
         self._check_arguments()
 
     def _check_arguments(self):
         """Check existence and consistency of argument values"""
         super()._check_arguments()
 
         if not self.input_format:
@@ -93,15 +90,17 @@
             )
             self.mapping_healpix_order = self.constant_healpix_order
         else:
             check_healpix_order_range(
                 self.highest_healpix_order, "highest_healpix_order"
             )
             if not 100 <= self.pixel_threshold <= 1_000_000_000:
-                raise ValueError("pixel_threshold should be between 100 and 1,000,000,000")
+                raise ValueError(
+                    "pixel_threshold should be between 100 and 1,000,000,000"
+                )
             self.mapping_healpix_order = self.highest_healpix_order
 
         if self.catalog_type not in ("source", "object"):
             raise ValueError("catalog_type should be one of `source` or `object`")
 
         if (not self.input_path and not self.input_file_list) or (
             self.input_path and self.input_file_list
@@ -113,36 +112,24 @@
         # Basic checks complete - make more checks and create directories where necessary
         if self.input_path:
             if not file_io.does_file_or_directory_exist(self.input_path):
                 raise FileNotFoundError("input_path not found on local storage")
             self.input_paths = file_io.find_files_matching_path(
                 self.input_path, f"*{self.input_format}"
             )
-
-            if len(self.input_paths) == 0:
-                raise FileNotFoundError(
-                    f"No files matched file pattern: {self.input_path}*{self.input_format} "
-                )
         elif self.input_file_list:
             self.input_paths = self.input_file_list
-            for test_path in self.input_paths:
-                if not file_io.does_file_or_directory_exist(test_path):
-                    raise FileNotFoundError(f"{test_path} not found on local storage")
-        self.input_paths.sort()
-
-        if not self.resume:
-            if file_io.directory_has_contents(self.tmp_path):
-                raise ValueError(
-                    f"tmp_path ({self.tmp_path}) contains intermediate files."
-                    " choose a different directory or use --resume flag"
-                )
-        file_io.make_directory(self.tmp_path, exist_ok=True)
-
-        if not self.filter_function:
-            self.filter_function = passthrough_filter_function
+        if len(self.input_paths) == 0:
+            raise FileNotFoundError("No input files found")
+        self.resume_plan = ResumePlan(
+            resume=self.resume,
+            progress_bar=self.progress_bar,
+            input_paths=self.input_paths,
+            tmp_path=self.tmp_path,
+        )
 
     def to_catalog_info(self, total_rows) -> CatalogInfo:
         """Catalog-type-specific dataset info."""
         info = {
             "catalog_name": self.output_catalog_name,
             "catalog_type": self.catalog_type,
             "total_rows": total_rows,
@@ -196,12 +183,7 @@
         raise ValueError(
             f"healpix order should be <= {hipscat_id.HIPSCAT_ID_HEALPIX_ORDER}"
         )
     if not lower_bound <= order <= upper_bound:
         raise ValueError(
             f"{field_name} should be between {lower_bound} and {upper_bound}"
         )
-
-
-def passthrough_filter_function(data: pd.DataFrame) -> pd.DataFrame:
-    """No-op filter function to be used when no user-defined filter is provided"""
-    return data
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import/catalog/file_readers.py` & `hipscat-import-0.0.5/src/hipscat_import/catalog/file_readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import abc
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 from astropy.table import Table
+from hipscat.io import file_io
 
 # pylint: disable=too-few-public-methods,too-many-arguments
 
 
 def get_file_reader(
     file_format,
     chunksize=500_000,
@@ -83,14 +84,27 @@
     def provenance_info(self) -> dict:
         """Create dictionary of parameters for provenance tracking.
 
         Returns:
             dictionary with all argument_name -> argument_value as key -> value pairs.
         """
 
+    def regular_file_exists(self, input_file):
+        """Check that the `input_file` points to a single regular file
+
+        Raises
+            FileNotFoundError: if nothing exists at path, or directory found.
+        """
+        if not file_io.does_file_or_directory_exist(input_file):
+            raise FileNotFoundError(f"File not found at path: {input_file}")
+        if not file_io.is_regular_file(input_file):
+            raise FileNotFoundError(
+                f"Directory found at path - requires regular file: {input_file}"
+            )
+
 
 class CsvReader(InputReader):
     """CSV reader for the most common CSV reading arguments.
 
     This uses `pandas.read_csv`, and you can find more information on
     additional arguments in the pandas documentation:
     https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
@@ -99,15 +113,16 @@
         chunksize (int): number of rows to read in a single iteration.
         header (int, list of int, None, default 'infer'): rows to
             use as the header with column names
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): the names of columns if no header is available
         type_map (dict): the data types to use for columns
-        separator (str): the character used for separation.
+        separator (str): the character used for separation. Use '\\s+' to
+            process whitespace separated files.
     """
 
     def __init__(
         self,
         chunksize=500_000,
         header="infer",
         schema_file=None,
@@ -121,14 +136,16 @@
         self.schema_file = schema_file
         self.column_names = column_names
         self.type_map = type_map
         self.separator = separator
         self.kwargs = kwargs
 
     def read(self, input_file):
+        self.regular_file_exists(input_file)
+
         if self.schema_file:
             schema_parquet = pd.read_parquet(
                 self.schema_file, dtype_backend="numpy_nullable"
             )
 
         use_column_names = None
         if self.column_names:
@@ -202,14 +219,15 @@
     ):
         self.chunksize = chunksize
         self.column_names = column_names
         self.skip_column_names = skip_column_names
         self.kwargs = kwargs
 
     def read(self, input_file):
+        self.regular_file_exists(input_file)
         table = Table.read(input_file, memmap=True, **self.kwargs)
         if self.column_names:
             table.keep_columns(self.column_names)
         elif self.skip_column_names:
             table.remove_columns(self.skip_column_names)
 
         total_rows = len(table)
@@ -239,14 +257,15 @@
     """
 
     def __init__(self, chunksize=500_000, **kwargs):
         self.chunksize = chunksize
         self.kwargs = kwargs
 
     def read(self, input_file):
+        self.regular_file_exists(input_file)
         parquet_file = pq.read_table(input_file, **self.kwargs)
         for smaller_table in parquet_file.to_batches(max_chunksize=self.chunksize):
             yield pa.Table.from_batches([smaller_table]).to_pandas()
 
     def provenance_info(self) -> dict:
         provenance_info = {
             "input_reader_type": "ParquetReader",
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import/catalog/map_reduce.py` & `hipscat-import-0.0.5/src/hipscat_import/catalog/map_reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import pyarrow as pa
 import pyarrow.parquet as pq
 from hipscat import pixel_math
 from hipscat.io import FilePointer, file_io, paths
 
 from hipscat_import.catalog.file_readers import InputReader
+from hipscat_import.catalog.resume_plan import ResumePlan
 
 # pylint: disable=too-many-locals,too-many-arguments
 
 
 def _get_pixel_directory(cache_path: FilePointer, order: np.int64, pixel: np.int64):
     """Create a path for intermediate pixel data.
 
@@ -50,53 +51,45 @@
 
 def _iterate_input_file(
     input_file: FilePointer,
     file_reader: InputReader,
     highest_order,
     ra_column,
     dec_column,
-    filter_function=None,
 ):
     """Helper function to handle input file reading and healpix pixel calculation"""
-    if not file_io.does_file_or_directory_exist(input_file):
-        raise FileNotFoundError(f"File not found at path: {input_file}")
-    if not file_io.is_regular_file(input_file):
-        raise FileNotFoundError(
-            f"Directory found at path - requires regular file: {input_file}"
-        )
     if not file_reader:
         raise NotImplementedError("No file reader implemented")
 
     required_columns = [ra_column, dec_column]
 
     for chunk_number, data in enumerate(file_reader.read(input_file)):
         if not all(x in data.columns for x in required_columns):
             raise ValueError(
                 f"Invalid column names in input file: {ra_column}, {dec_column} not in {input_file}"
             )
-        # Set up the data we want (filter and find pixel)
-        if filter_function:
-            data = filter_function(data)
+        # Set up the pixel data
         mapped_pixels = hp.ang2pix(
             2**highest_order,
             data[ra_column].values,
             data[dec_column].values,
             lonlat=True,
             nest=True,
         )
         yield chunk_number, data, mapped_pixels
 
 
 def map_to_pixels(
     input_file: FilePointer,
     file_reader: InputReader,
+    cache_path: FilePointer,
+    mapping_key,
     highest_order,
     ra_column,
     dec_column,
-    filter_function=None,
 ):
     """Map a file of input objects to their healpix pixels.
 
     Args:
         input_file (FilePointer): file to read for catalog data.
         file_reader (hipscat_import.catalog.file_readers.InputReader): instance of input
             reader that specifies arguments necessary for reading from the input file.
@@ -111,53 +104,52 @@
         to the number of objects found at the healpix pixel.
     Raises:
         ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
         FileNotFoundError: if the file does not exist, or is a directory
     """
     histo = pixel_math.empty_histogram(highest_order)
     for _, _, mapped_pixels in _iterate_input_file(
-        input_file, file_reader, highest_order, ra_column, dec_column, filter_function
+        input_file, file_reader, highest_order, ra_column, dec_column
     ):
         mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
         histo[mapped_pixel] += count_at_pixel.astype(np.int64)
-    return histo
+    ResumePlan.write_partial_histogram(
+        tmp_path=cache_path, mapping_key=mapping_key, histogram=histo
+    )
 
 
 def split_pixels(
     input_file: FilePointer,
     file_reader: InputReader,
     shard_suffix,
     highest_order,
     ra_column,
     dec_column,
     cache_path: FilePointer,
     alignment=None,
-    filter_function=None,
 ):
     """Map a file of input objects to their healpix pixels and split into shards.
 
     Args:
         input_file (FilePointer): file to read for catalog data.
         file_reader (hipscat_import.catalog.file_readers.InputReader): instance
             of input reader that specifies arguments necessary for reading from the input file.
         shard_suffix (str): unique counter for this input file, used
             when creating intermediate files
         highest_order (int): healpix order to use when mapping
         ra_column (str): where to find right ascension data in the dataframe
         dec_column (str): where to find declation in the dataframe
         cache_path (FilePointer): where to write intermediate files.
-        filter_function (function pointer): method to perform some filtering
-            or transformation of the input data
 
     Raises:
         ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
         FileNotFoundError: if the file does not exist, or is a directory
     """
     for chunk_number, data, mapped_pixels in _iterate_input_file(
-        input_file, file_reader, highest_order, ra_column, dec_column, filter_function
+        input_file, file_reader, highest_order, ra_column, dec_column
     ):
         aligned_pixels = alignment[mapped_pixels]
         unique_pixels, unique_inverse = np.unique(aligned_pixels, return_inverse=True)
 
         for unique_index, [order, pixel, _] in enumerate(unique_pixels):
             mapped_indexes = np.where(unique_inverse == unique_index)
             data_indexes = data.index[mapped_indexes[0].tolist()]
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import/catalog/run_import.py` & `hipscat-import-0.0.5/src/hipscat_import/catalog/run_import.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,123 +8,108 @@
 import hipscat.io.write_metadata as io
 import numpy as np
 from dask.distributed import as_completed
 from hipscat import pixel_math
 from tqdm import tqdm
 
 import hipscat_import.catalog.map_reduce as mr
-import hipscat_import.catalog.resume_files as resume
 from hipscat_import.catalog.arguments import ImportArguments
 
 
 def _map_pixels(args, client):
     """Generate a raw histogram of object counts in each healpix pixel"""
 
-    raw_histogram = resume.read_histogram(args.tmp_path, args.mapping_healpix_order)
-    if resume.is_mapping_done(args.tmp_path):
-        return raw_histogram
-
-    mapped_paths = set(resume.read_mapping_keys(args.tmp_path))
+    if args.resume_plan.is_mapping_done():
+        return
 
+    reader_future = client.scatter(args.file_reader)
     futures = []
-    for file_path in args.input_paths:
-        map_key = f"map_{file_path}"
-        if map_key in mapped_paths:
-            continue
+    for key, file_path in args.resume_plan.map_files:
         futures.append(
             client.submit(
                 mr.map_to_pixels,
-                key=map_key,
+                key=key,
                 input_file=file_path,
-                file_reader=args.file_reader,
-                filter_function=args.filter_function,
+                cache_path=args.tmp_path,
+                file_reader=reader_future,
+                mapping_key=key,
                 highest_order=args.mapping_healpix_order,
                 ra_column=args.ra_column,
                 dec_column=args.dec_column,
             )
         )
 
     some_error = False
-    for future, result in tqdm(
-        as_completed(futures, with_results=True),
+    for future in tqdm(
+        as_completed(futures),
         desc="Mapping  ",
         total=len(futures),
         disable=(not args.progress_bar),
     ):
         if future.status == "error":  # pragma: no cover
             some_error = True
-            continue
-        raw_histogram = np.add(raw_histogram, result)
-        resume.write_mapping_start_key(args.tmp_path, future.key)
-        resume.write_histogram(args.tmp_path, raw_histogram)
-        resume.write_mapping_done_key(args.tmp_path, future.key)
+        else:
+            args.resume_plan.mark_mapping_done(future.key)
     if some_error:  # pragma: no cover
         raise RuntimeError("Some mapping stages failed. See logs for details.")
-    resume.set_mapping_done(args.tmp_path)
-    return raw_histogram
+    args.resume_plan.set_mapping_done()
 
 
 def _split_pixels(args, alignment_future, client):
     """Generate a raw histogram of object counts in each healpix pixel"""
 
-    if resume.is_splitting_done(args.tmp_path):
+    if args.resume_plan.is_splitting_done():
         return
 
-    split_paths = set(resume.read_splitting_keys(args.tmp_path))
-
+    reader_future = client.scatter(args.file_reader)
     futures = []
-    for i, file_path in enumerate(args.input_paths):
-        split_key = f"split_{file_path}"
-        if split_key in split_paths:
-            continue
+    for key, file_path in args.resume_plan.split_keys:
         futures.append(
             client.submit(
                 mr.split_pixels,
-                key=split_key,
+                key=key,
                 input_file=file_path,
-                file_reader=args.file_reader,
-                filter_function=args.filter_function,
+                file_reader=reader_future,
                 highest_order=args.mapping_healpix_order,
                 ra_column=args.ra_column,
                 dec_column=args.dec_column,
-                shard_suffix=i,
+                shard_suffix=key,
                 cache_path=args.tmp_path,
                 alignment=alignment_future,
             )
         )
 
     some_error = False
     for future in tqdm(
         as_completed(futures),
         desc="Splitting",
         total=len(futures),
         disable=(not args.progress_bar),
     ):
         if future.status == "error":  # pragma: no cover
             some_error = True
-            continue
-        resume.write_splitting_done_key(args.tmp_path, future.key)
+        else:
+            args.resume_plan.mark_splitting_done(future.key)
     if some_error:  # pragma: no cover
         raise RuntimeError("Some splitting stages failed. See logs for details.")
-    resume.set_splitting_done(args.tmp_path)
+    args.resume_plan.set_splitting_done()
 
 
 def _reduce_pixels(args, destination_pixel_map, client):
     """Loop over destination pixels and merge into parquet files"""
 
-    if resume.is_reducing_done(args.tmp_path):
+    if args.resume_plan.is_reducing_done():
         return
 
-    reduced_keys = set(resume.read_reducing_keys(args.tmp_path))
-
     futures = []
-    for destination_pixel, source_pixels in destination_pixel_map.items():
-        destination_pixel_key = f"{destination_pixel.order}_{destination_pixel.pixel}"
-        if destination_pixel_key in reduced_keys:
-            continue
+    for (
+        destination_pixel,
+        source_pixels,
+        destination_pixel_key,
+    ) in args.resume_plan.get_reduce_items(destination_pixel_map):
         futures.append(
             client.submit(
                 mr.reduce_pixel_shards,
                 key=destination_pixel_key,
                 cache_path=args.tmp_path,
                 destination_pixel_order=destination_pixel.order,
                 destination_pixel_number=destination_pixel.pixel,
@@ -143,32 +128,34 @@
         as_completed(futures),
         desc="Reducing ",
         total=len(futures),
         disable=(not args.progress_bar),
     ):
         if future.status == "error":  # pragma: no cover
             some_error = True
-            continue
-        resume.write_reducing_key(args.tmp_path, future.key)
+        else:
+            args.resume_plan.mark_reducing_done(future.key)
     if some_error:  # pragma: no cover
         raise RuntimeError("Some reducing stages failed. See logs for details.")
-    resume.set_reducing_done(args.tmp_path)
+    args.resume_plan.set_reducing_done()
 
 
 def run(args, client):
     """Run catalog creation pipeline."""
     if not args:
         raise ValueError("args is required and should be type ImportArguments")
     if not isinstance(args, ImportArguments):
         raise ValueError("args must be type ImportArguments")
-    raw_histogram = _map_pixels(args, client)
+    _map_pixels(args, client)
 
     with tqdm(
-        total=1, desc="Binning  ", disable=not args.progress_bar
+        total=2, desc="Binning  ", disable=not args.progress_bar
     ) as step_progress:
+        raw_histogram = args.resume_plan.read_histogram(args.mapping_healpix_order)
+        step_progress.update(1)
         if args.constant_healpix_order >= 0:
             alignment = np.full(len(raw_histogram), None)
             for pixel_num, pixel_sum in enumerate(raw_histogram):
                 alignment[pixel_num] = (
                     args.constant_healpix_order,
                     pixel_num,
                     pixel_sum,
@@ -218,9 +205,9 @@
         io.write_fits_map(args.catalog_path, raw_histogram)
         step_progress.update(1)
         io.write_partition_info(
             catalog_base_dir=args.catalog_path,
             destination_healpix_pixel_map=destination_pixel_map,
         )
         step_progress.update(1)
-        resume.clean_resume_files(args.tmp_path)
+        args.resume_plan.clean_resume_files()
         step_progress.update(1)
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import/index/arguments.py` & `hipscat-import-0.0.5/src/hipscat_import/index/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/index/map_reduce.py` & `hipscat-import-0.0.5/src/hipscat_import/index/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/index/run_index.py` & `hipscat-import-0.0.5/src/hipscat_import/index/run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache.py` & `hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache_arguments.py` & `hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache_map_reduce.py` & `hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/src/hipscat_import/pipeline.py` & `hipscat-import-0.0.5/src/hipscat_import/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     """Pipeline that is run using an existing client.
 
     This can be useful in tests, or when a dask client requires some more complex
     configuraion.
     """
     try:
         if not args:
-            raise ValueError("args is required and should be subclass of RuntimeArguments")
+            raise ValueError(
+                "args is required and should be subclass of RuntimeArguments"
+            )
 
         if isinstance(args, ImportArguments):
             catalog_runner.run(args, client)
         elif isinstance(args, AssociationArguments):
             association_runner.run(args)
         elif isinstance(args, IndexArguments):
             index_runner.run(args)
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import/runtime_arguments.py` & `hipscat-import-0.0.5/src/hipscat_import/runtime_arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Data class to hold common runtime arguments for dataset creation."""
 
+from __future__ import annotations
+
 import re
 from dataclasses import dataclass
 from importlib.metadata import version
 
-from hipscat.io import file_io
+from hipscat.io import FilePointer, file_io
 
 # pylint: disable=too-many-instance-attributes
 
 
 @dataclass
 class RuntimeArguments:
     """Data class for holding runtime arguments"""
@@ -36,18 +38,18 @@
     dask_threads_per_worker: int = 1
     """number of threads per dask worker"""
 
     completion_email_address: str = ""
     """if provided, send an email to the indicated email address once the 
     import pipeline has complete."""
 
-    catalog_path = ""
+    catalog_path: FilePointer | None = None
     """constructed output path for the catalog that will be something like
     <output_path>/<output_catalog_name>"""
-    tmp_path = ""
+    tmp_path: FilePointer | None = None
     """constructed temp path - defaults to tmp_dir, then dask_tmp, but will create
     a new temp directory under catalog_path if no other options are provided"""
 
     def __post_init__(self):
         self._check_arguments()
 
     def _check_arguments(self):
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import.egg-info/PKG-INFO` & `hipscat-import-0.0.5/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.0.4
+Version: 0.0.5
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-import-0.0.4/src/hipscat_import.egg-info/SOURCES.txt` & `hipscat-import-0.0.5/src/hipscat_import.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 src/hipscat_import/association/arguments.py
 src/hipscat_import/association/map_reduce.py
 src/hipscat_import/association/run_association.py
 src/hipscat_import/catalog/__init__.py
 src/hipscat_import/catalog/arguments.py
 src/hipscat_import/catalog/file_readers.py
 src/hipscat_import/catalog/map_reduce.py
-src/hipscat_import/catalog/resume_files.py
+src/hipscat_import/catalog/resume_plan.py
 src/hipscat_import/catalog/run_import.py
 src/hipscat_import/index/__init__.py
 src/hipscat_import/index/arguments.py
 src/hipscat_import/index/map_reduce.py
 src/hipscat_import/index/run_index.py
 src/hipscat_import/margin_cache/__init__.py
 src/hipscat_import/margin_cache/margin_cache.py
@@ -71,15 +71,15 @@
 tests/hipscat_import/test_runtime_arguments.py
 tests/hipscat_import/association/test_association_argument.py
 tests/hipscat_import/association/test_association_map_reduce.py
 tests/hipscat_import/association/test_run_association.py
 tests/hipscat_import/catalog/test_argument_validation.py
 tests/hipscat_import/catalog/test_file_readers.py
 tests/hipscat_import/catalog/test_map_reduce.py
-tests/hipscat_import/catalog/test_resume_files.py
+tests/hipscat_import/catalog/test_resume_plan.py
 tests/hipscat_import/catalog/test_run_import.py
 tests/hipscat_import/catalog/test_run_round_trip.py
 tests/hipscat_import/data/blank/blank.csv
 tests/hipscat_import/data/mixed_schema/input_01.csv
 tests/hipscat_import/data/mixed_schema/input_02.csv
 tests/hipscat_import/data/mixed_schema/schema.parquet
 tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
```

### Comparing `hipscat-import-0.0.4/tests/.pylintrc` & `hipscat-import-0.0.5/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/association/test_association_argument.py` & `hipscat-import-0.0.5/tests/hipscat_import/association/test_association_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/association/test_association_map_reduce.py` & `hipscat-import-0.0.5/tests/hipscat_import/association/test_association_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/association/test_run_association.py` & `hipscat-import-0.0.5/tests/hipscat_import/association/test_run_association.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_argument_validation.py` & `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_argument_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,24 +62,14 @@
             output_catalog_name="catalog",
             input_path=blank_data_dir,
             output_path=tmp_path,
             overwrite=True,
             input_format="parquet",
         )
 
-    ## Bad input file
-    with pytest.raises(FileNotFoundError):
-        ImportArguments(
-            output_catalog_name="catalog",
-            input_file_list=["/foo/path"],
-            overwrite=True,
-            output_path=tmp_path,
-            input_format="csv",
-        )
-
 
 def test_good_paths(blank_data_dir, blank_data_file, tmp_path):
     """Required arguments are provided, and paths are found."""
     tmp_path_str = str(tmp_path)
     args = ImportArguments(
         output_catalog_name="catalog",
         input_path=blank_data_dir,
```

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_file_readers.py` & `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_map_reduce.py` & `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_map_reduce.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,76 +4,96 @@
 
 import hipscat.pixel_math as hist
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pyarrow as pa
 import pytest
+from numpy import frombuffer
 
 import hipscat_import.catalog.map_reduce as mr
 from hipscat_import.catalog.file_readers import get_file_reader
 
 
 def test_read_empty_filename():
     """Empty file name"""
     with pytest.raises(FileNotFoundError):
         mr.map_to_pixels(
             input_file="",
             file_reader=get_file_reader("parquet"),
             highest_order=10,
             ra_column="ra",
             dec_column="dec",
+            cache_path="",
+            mapping_key="map_0",
         )
 
 
 def test_read_wrong_fileformat(small_sky_file0):
     """CSV file attempting to be read as parquet"""
     with pytest.raises(pa.lib.ArrowInvalid):
         mr.map_to_pixels(
             input_file=small_sky_file0,
             file_reader=get_file_reader("parquet"),
             highest_order=0,
             ra_column="ra_mean",
             dec_column="dec_mean",
+            cache_path="",
+            mapping_key="map_0",
         )
 
 
 def test_read_directory(test_data_dir):
     """Provide directory, not file"""
     with pytest.raises(FileNotFoundError):
         mr.map_to_pixels(
             input_file=test_data_dir,
             file_reader=get_file_reader("parquet"),
             highest_order=0,
             ra_column="ra",
             dec_column="dec",
+            cache_path="",
+            mapping_key="map_0",
         )
 
 
 def test_read_bad_fileformat(blank_data_file):
     """Unsupported file format"""
     with pytest.raises(NotImplementedError):
         mr.map_to_pixels(
             input_file=blank_data_file,
             file_reader=None,
             highest_order=0,
             ra_column="ra",
             dec_column="dec",
+            cache_path="",
+            mapping_key="map_0",
         )
 
 
-def test_read_single_fits(formats_fits):
+def read_partial_histogram(tmp_path, mapping_key):
+    """Helper to read in the former result of a map operation."""
+    histogram_file = os.path.join(tmp_path, "histograms", f"{mapping_key}.binary")
+    with open(histogram_file, "rb") as file_handle:
+        return frombuffer(file_handle.read(), dtype=np.int64)
+
+
+def test_read_single_fits(tmp_path, formats_fits):
     """Success case - fits file that exists being read as fits"""
-    result = mr.map_to_pixels(
+    mr.map_to_pixels(
         input_file=formats_fits,
         file_reader=get_file_reader("fits"),
         highest_order=0,
         ra_column="ra",
         dec_column="dec",
+        cache_path=tmp_path,
+        mapping_key="map_0",
     )
+
+    result = read_partial_histogram(tmp_path, "map_0")
     assert len(result) == 12
     expected = hist.empty_histogram(0)
     expected[11] = 131
     npt.assert_array_equal(result, expected)
 
 
 def test_map_headers_wrong(formats_headers_csv):
@@ -81,102 +101,116 @@
     with pytest.raises(ValueError, match="header"):
         mr.map_to_pixels(
             input_file=formats_headers_csv,
             file_reader=get_file_reader("csv"),
             highest_order=0,
             ra_column="ra",
             dec_column="dec",
+            cache_path="",
+            mapping_key="map_0",
         )
 
 
-def test_map_headers(formats_headers_csv):
+def test_map_headers(tmp_path, formats_headers_csv):
     """Test loading the a file with non-default headers"""
-    result = mr.map_to_pixels(
+    mr.map_to_pixels(
         input_file=formats_headers_csv,
         file_reader=get_file_reader("csv"),
         highest_order=0,
         ra_column="ra_mean",
         dec_column="dec_mean",
+        cache_path=tmp_path,
+        mapping_key="map_0",
     )
 
+    result = read_partial_histogram(tmp_path, "map_0")
+
     assert len(result) == 12
 
     expected = hist.empty_histogram(0)
     expected[11] = 8
     npt.assert_array_equal(result, expected)
     assert (result == expected).all()
 
 
-def test_split_pixels_headers(formats_headers_csv, assert_parquet_file_ids, tmp_path):
-    """Test loading the a file with non-default headers"""
-    alignment = np.full(12, None)
-    alignment[11] = (0, 11, 131)
-    mr.split_pixels(
-        input_file=formats_headers_csv,
-        file_reader=get_file_reader("csv"),
-        highest_order=0,
-        ra_column="ra_mean",
-        dec_column="dec_mean",
-        shard_suffix=0,
-        cache_path=tmp_path,
-        alignment=alignment,
-    )
-
-    file_name = os.path.join(
-        tmp_path, "order_0", "dir_0", "pixel_11", "shard_0_0.parquet"
-    )
-    expected_ids = [*range(700, 708)]
-    assert_parquet_file_ids(file_name, "object_id", expected_ids)
-
-    file_name = os.path.join(
-        tmp_path, "order_0", "dir_0", "pixel_1", "shard_0_0.parquet"
-    )
-    assert not os.path.exists(file_name)
-
-
-def test_map_small_sky_order0(small_sky_single_file):
+def test_map_small_sky_order0(tmp_path, small_sky_single_file):
     """Test loading the small sky catalog and partitioning each object into the same large bucket"""
-    result = mr.map_to_pixels(
+    mr.map_to_pixels(
         input_file=small_sky_single_file,
         file_reader=get_file_reader("csv"),
         highest_order=0,
         ra_column="ra",
         dec_column="dec",
+        cache_path=tmp_path,
+        mapping_key="map_0",
     )
 
+    result = read_partial_histogram(tmp_path, "map_0")
+
     assert len(result) == 12
 
     expected = hist.empty_histogram(0)
     expected[11] = 131
     npt.assert_array_equal(result, expected)
     assert (result == expected).all()
 
 
-def test_map_small_sky_part_order1(small_sky_file0):
+def test_map_small_sky_part_order1(tmp_path, small_sky_file0):
     """
     Test loading a small portion of the small sky catalog and
     partitioning objects into four smaller buckets
     """
-    result = mr.map_to_pixels(
+    mr.map_to_pixels(
         input_file=small_sky_file0,
         file_reader=get_file_reader("csv"),
         highest_order=1,
         ra_column="ra",
         dec_column="dec",
+        cache_path=tmp_path,
+        mapping_key="map_0",
     )
 
+    result = read_partial_histogram(tmp_path, "map_0")
+
     assert len(result) == 48
 
     expected = hist.empty_histogram(1)
     filled_pixels = [5, 7, 11, 2]
     expected[44:] = filled_pixels[:]
     npt.assert_array_equal(result, expected)
     assert (result == expected).all()
 
 
+def test_split_pixels_headers(formats_headers_csv, assert_parquet_file_ids, tmp_path):
+    """Test loading the a file with non-default headers"""
+    alignment = np.full(12, None)
+    alignment[11] = (0, 11, 131)
+    mr.split_pixels(
+        input_file=formats_headers_csv,
+        file_reader=get_file_reader("csv"),
+        highest_order=0,
+        ra_column="ra_mean",
+        dec_column="dec_mean",
+        shard_suffix=0,
+        cache_path=tmp_path,
+        alignment=alignment,
+    )
+
+    file_name = os.path.join(
+        tmp_path, "order_0", "dir_0", "pixel_11", "shard_0_0.parquet"
+    )
+    expected_ids = [*range(700, 708)]
+    assert_parquet_file_ids(file_name, "object_id", expected_ids)
+
+    file_name = os.path.join(
+        tmp_path, "order_0", "dir_0", "pixel_1", "shard_0_0.parquet"
+    )
+    assert not os.path.exists(file_name)
+
+
 def test_reduce_order0(parquet_shards_dir, assert_parquet_file_ids, tmp_path):
     """Test reducing into one large pixel"""
     mr.reduce_pixel_shards(
         cache_path=parquet_shards_dir,
         destination_pixel_order=0,
         destination_pixel_number=11,
         destination_pixel_size=131,
```

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_import.py` & `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Functional tests for catalog import"""
 
 import os
 import shutil
 
+import hipscat.pixel_math as hist
 import pytest
 from hipscat.catalog.catalog import Catalog
 
-import hipscat_import.catalog.resume_files as rf
 import hipscat_import.catalog.run_import as runner
 from hipscat_import.catalog.arguments import ImportArguments
+from hipscat_import.catalog.resume_plan import ResumePlan
 
 
 def test_empty_args():
     """Runner should fail with empty arguments"""
     with pytest.raises(ValueError, match="args is required"):
         runner.run(None, None)
 
@@ -36,26 +37,25 @@
     ## First, copy over our intermediate files.
     ## This prevents overwriting source-controlled resume files.
     temp_path = os.path.join(tmp_path, "resume", "intermediate")
     shutil.copytree(
         os.path.join(resume_dir, "intermediate"),
         temp_path,
     )
+    plan = ResumePlan(tmp_path=temp_path, progress_bar=False, resume=True)
+    histogram = hist.empty_histogram(0)
+    histogram[11] = 131
+    empty = hist.empty_histogram(0)
     for file_index in range(0, 5):
-        rf.write_mapping_start_key(
-            temp_path,
-            f"map_{os.path.join(small_sky_parts_dir, f'catalog_0{file_index}_of_05.csv')}",
-        )
-        rf.write_mapping_done_key(
-            temp_path,
-            f'map_{os.path.join(small_sky_parts_dir, f"catalog_0{file_index}_of_05.csv")}',
-        )
-        rf.write_splitting_done_key(
-            temp_path,
-            f'split_{os.path.join(small_sky_parts_dir, f"catalog_0{file_index}_of_05.csv")}',
+        plan.mark_mapping_done(f"map_{file_index}")
+        plan.mark_splitting_done(f"split_{file_index}")
+        ResumePlan.write_partial_histogram(
+            tmp_path=temp_path,
+            mapping_key=f"map_{file_index}",
+            histogram=histogram if file_index == 0 else empty,
         )
 
     shutil.copytree(
         os.path.join(resume_dir, "Norder=0"),
         os.path.join(tmp_path, "resume", "Norder=0"),
     )
 
@@ -109,17 +109,18 @@
 
     ## Re-running the pipeline with fully done intermediate files
     ## should result in no changes to output files.
     shutil.copytree(
         os.path.join(resume_dir, "intermediate"),
         temp_path,
     )
-    rf.set_mapping_done(temp_path)
-    rf.set_splitting_done(temp_path)
-    rf.set_reducing_done(temp_path)
+    plan = args.resume_plan
+    plan.set_mapping_done()
+    plan.set_splitting_done()
+    plan.set_reducing_done()
 
     args = ImportArguments(
         output_catalog_name="resume",
         input_path=small_sky_parts_dir,
         input_format="csv",
         output_path=tmp_path,
         dask_tmp=tmp_path,
```

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_round_trip.py` & `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_round_trip.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,14 +316,15 @@
     )
 
     data_frame = pd.read_parquet(output_file, engine="pyarrow")
     assert len(data_frame) == 14
     ids = data_frame["id"]
     assert np.logical_and(ids >= 700, ids < 832).all()
 
+
 @pytest.mark.dask
 def test_import_starr_file(
     dask_client,
     formats_dir,
     assert_parquet_file_ids,
     tmp_path,
 ):
@@ -331,17 +332,25 @@
     - tests that we can run pipeline with a totally unknown file type, so long
       as a valid InputReader implementation is provided.
     """
 
     class StarrReader(CsvReader):
         """Shallow subclass"""
 
+        def read(self, input_file):
+            import glob
+
+            files = glob.glob(f"{input_file}/**.starr")
+            files.sort()
+            for file in files:
+                return super().read(file)
+
     args = ImportArguments(
         output_catalog_name="starr",
-        input_path=formats_dir,
+        input_file_list=[formats_dir],
         input_format="starr",
         file_reader=StarrReader(),
         output_path=tmp_path,
         dask_tmp=tmp_path,
         highest_healpix_order=2,
         pixel_threshold=3_000,
         progress_bar=False,
@@ -358,8 +367,8 @@
 
     # Check that the catalog parquet file exists and contains correct object IDs
     output_file = os.path.join(
         args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
     )
 
     expected_ids = [*range(700, 831)]
-    assert_parquet_file_ids(output_file, "id", expected_ids)
+    assert_parquet_file_ids(output_file, "id", expected_ids)
```

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/conftest.py` & `hipscat-import-0.0.5/tests/hipscat_import/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,76 +160,79 @@
     return os.path.join(test_data_dir, "mixed_schema", "schema.parquet")
 
 
 @pytest.fixture
 def resume_dir(test_data_dir):
     return os.path.join(test_data_dir, "resume")
 
+
 @pytest.fixture
 def basic_data_shard_df():
-    ras = np.arange(0.,360.)
-    dec = np.full(360, 0.)
+    ras = np.arange(0.0, 360.0)
+    dec = np.full(360, 0.0)
     ppix = np.full(360, 21)
     porder = np.full(360, 1)
     norder = np.full(360, 1)
     npix = np.full(360, 0)
 
     test_df = pd.DataFrame(
         data=zip(ras, dec, ppix, porder, norder, npix),
         columns=[
-            "weird_ra", 
+            "weird_ra",
             "weird_dec",
             "partition_pixel",
             "partition_order",
             "Norder",
-            "Npix"
-        ]
+            "Npix",
+        ],
     )
 
     test_df["margin_pixel"] = hp.ang2pix(
         2**3,
         test_df["weird_ra"].values,
         test_df["weird_dec"].values,
         lonlat=True,
-        nest=True
+        nest=True,
     )
 
     return test_df
 
+
 @pytest.fixture
 def polar_data_shard_df():
-    ras = np.arange(0.,360.)
+    ras = np.arange(0.0, 360.0)
     dec = np.full(360, 89.9)
     ppix = np.full(360, 15)
     porder = np.full(360, 2)
     norder = np.full(360, 2)
     npix = np.full(360, 0)
 
     test_df = pd.DataFrame(
         data=zip(ras, dec, ppix, porder, norder, npix),
         columns=[
-            "weird_ra", 
+            "weird_ra",
             "weird_dec",
             "partition_pixel",
             "partition_order",
             "Norder",
-            "Npix"
-        ]
+            "Npix",
+        ],
     )
 
     test_df["margin_pixel"] = hp.ang2pix(
         2**3,
         test_df["weird_ra"].values,
         test_df["weird_dec"].values,
         lonlat=True,
-        nest=True
+        nest=True,
     )
 
     return test_df
 
+
 @pytest.fixture
 def assert_text_file_matches():
     def assert_text_file_matches(expected_lines, file_name):
         """Convenience method to read a text file and compare the contents, line for line.
 
         When file contents get even a little bit big, it can be difficult to see
         the difference between an actual file and the expected contents without
```

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_metadata` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source/small_sky_source.csv` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source/small_sky_source.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/_metadata` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json` & `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/catalog.starr` & `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/catalog.starr`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/multiindex.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/multiindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/pandasindex.parquet` & `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/pandasindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/small_sky.fits` & `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/small_sky.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/index/test_index_argument.py` & `hipscat-import-0.0.5/tests/hipscat_import/index/test_index_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/index/test_index_map_reduce.py` & `hipscat-import-0.0.5/tests/hipscat_import/index/test_index_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/index/test_run_index.py` & `hipscat-import-0.0.5/tests/hipscat_import/index/test_run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py` & `hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_margin_cache.py` & `hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py` & `hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.4/tests/hipscat_import/test_runtime_arguments.py` & `hipscat-import-0.0.5/tests/hipscat_import/test_runtime_arguments.py`

 * *Files identical despite different names*

