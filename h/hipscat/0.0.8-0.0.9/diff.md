# Comparing `tmp/hipscat-0.0.8.tar.gz` & `tmp/hipscat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.0.8.tar", last modified: Wed Mar 29 17:02:28 2023, max compression
+gzip compressed data, was "hipscat-0.0.9.tar", last modified: Thu Apr 13 18:52:35 2023, max compression
```

## Comparing `hipscat-0.0.8.tar` & `hipscat-0.0.9.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.141479 hipscat-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-29 17:02:09.000000 hipscat-0.0.8/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.125479 hipscat-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.129479 hipscat-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-29 17:02:09.000000 hipscat-0.0.8/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-29 17:02:09.000000 hipscat-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-29 17:02:09.000000 hipscat-0.0.8/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-29 17:02:09.000000 hipscat-0.0.8/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-29 17:02:09.000000 hipscat-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-03-29 17:02:09.000000 hipscat-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-29 17:02:09.000000 hipscat-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-29 17:02:09.000000 hipscat-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-29 17:02:28.141479 hipscat-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-29 17:02:09.000000 hipscat-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-29 17:02:09.000000 hipscat-0.0.8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.129479 hipscat-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.129479 hipscat-0.0.8/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.129479 hipscat-0.0.8/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-29 17:02:09.000000 hipscat-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.129479 hipscat-0.0.8/nb/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-29 17:02:09.000000 hipscat-0.0.8/nb/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-03-29 17:02:09.000000 hipscat-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 17:02:28.141479 hipscat-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.133479 hipscat-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.133479 hipscat-0.0.8/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-29 17:02:27.000000 hipscat-0.0.8/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.133479 hipscat-0.0.8/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/catalog_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/partition_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/pixel_node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/catalog/pixel_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.133479 hipscat-0.0.8/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.133479 hipscat-0.0.8/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/pixel_math/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-03-29 17:02:09.000000 hipscat-0.0.8/src/hipscat/pixel_math/pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.133479 hipscat-0.0.8/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-29 17:02:28.000000 hipscat-0.0.8/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-29 17:02:28.000000 hipscat-0.0.8/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 17:02:28.000000 hipscat-0.0.8/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-29 17:02:28.000000 hipscat-0.0.8/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-29 17:02:28.000000 hipscat-0.0.8/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.125479 hipscat-0.0.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.125479 hipscat-0.0.8/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky/point_map.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.125479 hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.137479 hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/data/small_sky_order1/point_map.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.129479 hipscat-0.0.8/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.141479 hipscat-0.0.8/tests/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/catalog/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/catalog/test_catalog_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/catalog/test_pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/catalog/test_pixel_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.141479 hipscat-0.0.8/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.141479 hipscat-0.0.8/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.141479 hipscat-0.0.8/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:28.141479 hipscat-0.0.8/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-03-29 17:02:09.000000 hipscat-0.0.8/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.544044 hipscat-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 18:52:25.000000 hipscat-0.0.9/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.512043 hipscat-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.524043 hipscat-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 18:52:25.000000 hipscat-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-13 18:52:25.000000 hipscat-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 18:52:25.000000 hipscat-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 18:52:25.000000 hipscat-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-13 18:52:35.540044 hipscat-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 18:52:25.000000 hipscat-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 18:52:25.000000 hipscat-0.0.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.524043 hipscat-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/nb/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 18:52:25.000000 hipscat-0.0.9/nb/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-13 18:52:25.000000 hipscat-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:52:35.544044 hipscat-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/catalog_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/pixel_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/pixel_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.532044 hipscat-0.0.9/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.516044 hipscat-0.0.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.516044 hipscat-0.0.9/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/point_map.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.516044 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/point_map.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.520043 hipscat-0.0.9/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_catalog_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_pixel_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_pixel_margins.py
```

### Comparing `hipscat-0.0.8/.github/workflows/linting.yml` & `hipscat-0.0.9/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/.github/workflows/publish-to-pypi.yml` & `hipscat-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/.github/workflows/smoke-test.yml` & `hipscat-0.0.9/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/.github/workflows/testing-and-coverage.yml` & `hipscat-0.0.9/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/.gitignore` & `hipscat-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/.pre-commit-config.yaml` & `hipscat-0.0.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 repos:
 
+    # Compare the local template version to the latest remote template version
+    # This hook should always pass. It will print a message if the local version 
+    # is out of date.
+  - repo: https://github.com/lincc-frameworks/pre-commit-hooks
+    rev: v0.1
+    hooks:
+      - id: check-lincc-frameworks-template-version
+        name: Check template version
+        description: Compare current template version against latest
+        verbose: true
+
     # Clear output from jupyter notebooks so that only the input cells are committed.
   - repo: local
     hooks:
       - id: jupyter-nb-clear-output
         name: jupyter-nb-clear-output
         description: Clear output from Jupyter notebooks.
         files: \.ipynb$
@@ -53,15 +64,15 @@
       - id: isort
         name: isort (python files in src/ and tests/)
         description: Sort and organize imports in .py files.
         types: [python]
         files: ^(src|tests)/
 
 
-      # Analyze the src code style and report code that doesn't adhere.
+    # Analyze the src code style and report code that doesn't adhere.
   - repo: local
     hooks:
       - id: pylint
         name: pylint (python files in src/)
         entry: pylint
         language: system
         types: [python]
```

### Comparing `hipscat-0.0.8/LICENSE` & `hipscat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/PKG-INFO` & `hipscat-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.0.8
+Version: 0.0.9
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Astronomy Data Commons
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-0.0.8/README.md` & `hipscat-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/docs/conf.py` & `hipscat-0.0.9/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,11 +38,12 @@
 # Remove 'view source code' from top of page (for html, not python)
 html_show_sourcelink = False
 # Remove namespaces from class/method signatures
 add_module_names = False
 
 autoapi_type = "python"
 autoapi_dirs = ["../src"]
+autoapi_ignore = ["*/__main__.py", "*/_version.py"]
 autoapi_add_toc_tree_entry = False
 autoapi_member_order = "bysource"
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `hipscat-0.0.8/docs/guide/contributing.rst` & `hipscat-0.0.9/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/docs/guide/directory_scheme.rst` & `hipscat-0.0.9/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/nb/example.ipynb` & `hipscat-0.0.9/nb/example.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/pyproject.toml` & `hipscat-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 
 requires-python = ">=3.8"
 dependencies = [
     "healpy",
     "pandas",
     "setuptools_scm",
     "pyarrow",
+    "astropy",
+    "regions"
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "mypy", # Used for static type checking of files
     "pylint", # Used for static linting of files
     "pre-commit", # Used to run checks before finalizing a git commit
     "pytest",
     "pytest-cov", # Used to report total code coverage
+    "pytest-timeout", # Used to test for code efficiency
     "sphinx==6.1.3", # Used to automatically generate documentation
     "sphinx_rtd_theme==1.2.0", # Used to render documentation
     "sphinx-autoapi==2.0.1", # Used to automatically generate api documentation
 ]
 [metadata]
 description = "Hierarchical Progressive Survey Catalog"
 long_description = { file = "README.md" }
@@ -45,7 +48,10 @@
     "setuptools>=45", # Used to build and package the Python project
     "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/hipscat/_version.py"
+
+[tool.coverage.run]
+omit=["src/hipscat/_version.py"]
```

### Comparing `hipscat-0.0.8/src/.pylintrc` & `hipscat-0.0.9/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/catalog/catalog.py` & `hipscat-0.0.9/src/hipscat/catalog/catalog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 """Container class to hold catalog metadata and partition iteration"""
 
 
+from hipscat.catalog.catalog_parameters import read_from_metadata_file
 from hipscat.catalog.partition_info import PartitionInfo
 from hipscat.io import file_io, paths
 
 
 class Catalog:
     """Container class for catalog metadata"""
 
     def __init__(self, catalog_path: str = None) -> None:
         self.catalog_path = catalog_path
         self.catalog_base_dir = file_io.get_file_pointer_from_path(catalog_path)
         self.metadata_keywords = None
 
         self.partition_info = None
+        self.catalog_info = None
 
         self.catalog_name = None
+        self.catalog_type = None
 
         self._initialize_metadata()
 
     def _initialize_metadata(self):
         if not file_io.does_file_or_directory_exist(self.catalog_base_dir):
             raise FileNotFoundError(
                 f"No directory exists at {str(self.catalog_base_dir)}"
             )
         catalog_info_file = paths.get_catalog_info_pointer(self.catalog_base_dir)
         if not file_io.does_file_or_directory_exist(catalog_info_file):
             raise FileNotFoundError(
                 f"No catalog info found where expected: {str(catalog_info_file)}"
             )
+        self.catalog_info = read_from_metadata_file(catalog_info_file)
+        self.catalog_name = self.catalog_info.catalog_name
+        self.catalog_type = self.catalog_info.catalog_type
 
-        self.metadata_keywords = file_io.load_json_file(catalog_info_file)
-        self.catalog_name = self.metadata_keywords["catalog_name"]
-        self.partition_info = PartitionInfo(self.catalog_base_dir)
+        if self.catalog_type in ("object", "source"):
+            self.partition_info = PartitionInfo(self.catalog_base_dir)
 
     def get_pixels(self):
         """Get all healpix pixels that are contained in the catalog
 
         Returns:
             data frame with per-pixel data.
```

### Comparing `hipscat-0.0.8/src/hipscat/catalog/pixel_node.py` & `hipscat-0.0.9/src/hipscat/catalog/pixel_node.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/catalog/pixel_tree.py` & `hipscat-0.0.9/src/hipscat/catalog/pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.0.9/src/hipscat/inspection/visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/io/file_io/file_io.py` & `hipscat-0.0.9/src/hipscat/io/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.0.9/src/hipscat/io/file_io/file_pointer.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.0.9/src/hipscat/pixel_math/hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.0.9/src/hipscat/pixel_math/pixel_margins.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,156 +1,183 @@
-"""Utilities for generating and manipulating object count histograms"""
+"""Utilities for find the pixels of higher orders that surround a given healpixel."""
 
 import healpy as hp
 import numpy as np
-import pandas as pd
 
-
-def empty_histogram(highest_order):
-    """Use numpy to create an histogram array with the right shape, filled with zeros.
+# see the documentation for get_edge() about this variable
+_edge_vectors = [
+    np.asarray([1, 3]),  # NE edge
+    np.asarray([1]),  # E corner
+    np.asarray([0, 1]),  # SE edge
+    np.asarray([0]),  # S corner
+    np.asarray([0, 2]),  # SW edge
+    np.asarray([2]),  # W corner
+    np.asarray([2, 3]),  # NW edge
+    np.asarray([3]),  # N corner
+]
+
+# cache used by get_margin()
+_suffixes = {}
+
+
+def get_edge(d_order, pix, edge):
+    """Get all the pixels at order kk+dk bordering pixel pix.
+    See hipscat/pixel_math/README.md for more info.
 
     Args:
-        highest_order (int): the highest healpix order (e.g. 0-10)
+        dk (int): the change in k that we wish to find the margins for.
+        pix (int): the healpix pixel to find margin pixels of.
+        edge (int): the edge we want to find for the given pixel. (0-7)
+            0: NE edge
+            1: E corner
+            2: SE edge
+            3: S corner
+            4: SW edge
+            5: W corner
+            6: NW edge
+            7: N corner
     Returns:
-        one-dimensional numpy array of long integers, where the length is equal to
-        the number of pixels in a healpix map of target order, and all values are set to 0.
+        one-dimensional numpy array of long integers, filled with the healpix pixels
+            at order kk+dk that border the given edge of pix.
     """
-    return np.zeros(hp.order2npix(highest_order), dtype=np.int64)
-
+    if edge < 0 or edge > 7:
+        raise ValueError("edge can only be values between 0 and 7 (see docstring)")
 
-def generate_histogram(
-    data: pd.DataFrame,
-    highest_order,
-    ra_column="ra",
-    dec_column="dec",
-):
-    """Generate a histogram of counts for objects found in `data`
+    if (edge, d_order) in _suffixes:
+        pixel_edge = _suffixes[(edge, d_order)]
+    else:
+        # generate and cache the suffix:
+
+        # generate all combinations of i,j,k,... suffixes for the requested edge
+        # See https://stackoverflow.com/a/35608701
+        grid = np.array(np.meshgrid(*[_edge_vectors[edge]] * d_order))
+        pixel_edge = grid.T.reshape(-1, d_order)
+        # bit-shift each suffix by the required number of bits
+        pixel_edge <<= np.arange(2 * (d_order - 1), -2, -2)
+        # sum them up row-wise, generating the suffix
+        pixel_edge = pixel_edge.sum(axis=1)
+        # cache for further reuse
+        _suffixes[(edge, d_order)] = pixel_edge
+
+    # append the 'pix' preffix
+    pixel_edge = (pix << 2 * d_order) + pixel_edge
+    return pixel_edge
+
+
+def get_margin(order, pix, d_order):
+    """Get all the pixels at order order+dk bordering pixel pix.
+    See hipscat/pixel_math/README.md for more info.
 
     Args:
-        data (obj:`pd.DataFrame`): tabular object data
-        highest_order (int):  the highest healpix order (e.g. 0-10)
-        ra_column (str): where in the input to find the celestial coordinate, right ascension
-        dec_column (str): where in the input to find the celestial coordinate, declination
+        order (int): the healpix order of pix.
+        pix (int): the healpix pixel to find margin pixels of.
+        d_order (int): the change in k that we wish to find the margins for.
+            Must be greater than kk.
     Returns:
-        one-dimensional numpy array of long integers where the value at each index corresponds
-        to the number of objects found at the healpix pixel.
-    Raises:
-        ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
+        one-dimensional numpy array of long integers, filled with the healpix pixels
+            at order kk+dk that border pix.
     """
-    histogram_result = empty_histogram(highest_order)
+    if d_order < 1:
+        raise ValueError("dk must be greater than order")
 
-    # Verify that the data frame has columns with desired names.
-    required_columns = [ra_column, dec_column]
-    if not all(x in data.columns for x in required_columns):
-        raise ValueError(f"Invalid column names in input: {ra_column}, {dec_column}")
-    mapped_pixels = hp.ang2pix(
-        2**highest_order,
-        data[ra_column].values,
-        data[dec_column].values,
-        lonlat=True,
-        nest=True,
-    )
-    mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
-    histogram_result[mapped_pixel] += count_at_pixel.astype(np.int64)
-    return histogram_result
-
-
-def generate_alignment(histogram, highest_order=10, threshold=1_000_000):
-    """Generate alignment from high order pixels to those of equal or lower order
-
-    We may initially find healpix pixels at order 10, but after aggregating up to the pixel
-    threshold, some final pixels are order 4 or 7. This method provides a map from pixels
-    at order 10 to their destination pixel. This may be used as an input into later partitioning
-    map reduce steps.
+    nside = hp.order2nside(order)
 
-    Args:
-        histogram (:obj:`np.array`): one-dimensional numpy array of long integers where the
-            value at each index corresponds to the number of objects found at the healpix pixel.
-        highest_order (int):  the highest healpix order (e.g. 0-10)
-        threshold (int): the maximum number of objects allowed in a single pixel
-    Returns:
-        one-dimensional numpy array of integer 3-tuples, where the value at each index corresponds
-        to the destination pixel at order less than or equal to the `highest_order`.
-
-        The tuple contains three integers:
-
-        - order of the destination pixel
-        - pixel number *at the above order*
-        - the number of objects in the pixel
-    """
+    # get all neighboring pixels
+    neighbors = hp.get_all_neighbours(nside, pix, nest=True)
 
-    if len(histogram) != hp.order2npix(highest_order):
-        raise ValueError("histogram is not the right size")
+    # get the healpix faces IDs of pix and the neighboring pixels
+    _, _, pix_face = hp.pix2xyf(nside, pix, nest=True)
+    _, _, faces = hp.pix2xyf(nside, neighbors, nest=True)
+
+    # indices which tell get_edge() which edge/verted to return
+    # for a given pixel. The default order is compatible with the
+    # order returned by hp.get_all_neighbours().
+    which = np.arange(8)
+
+    # northern hemisphere; 90deg cw rotation for every +1 face increment
+    if pix_face < 4:
+        mask = faces < 4
+        which[mask] += 2 * (faces - pix_face)[mask]
+        which %= 8
+    # southern hemisphere; 90deg ccw rotation for every +1 face increment
+    elif pix_face >= 8:
+        mask = faces >= 8
+        which[mask] -= 2 * (faces - pix_face)[mask]
+        which %= 8
+
+    # get all edges/vertices
+    # (making sure we skip -1 entries, for pixels with seven neighbors)
+    margins = []
+    for edge, pixel in zip(which, neighbors):
+        if pixel != -1:
+            margins.append(get_edge(d_order, pixel, edge))
+    margins = np.concatenate(margins)
+    return margins
 
-    nested_sums = []
-    for i in range(0, highest_order):
-        nested_sums.append(empty_histogram(i))
-    nested_sums.append(histogram)
-
-    # work backward - from highest order, fill in the sums of lower order pixels
-    for read_order in range(highest_order, 0, -1):
-        parent_order = read_order - 1
-        for index in range(0, len(nested_sums[read_order])):
-            parent_pixel = index >> 2
-            nested_sums[parent_order][parent_pixel] += nested_sums[read_order][index]
-
-    nested_alignment = []
-    for i in range(0, highest_order + 1):
-        nested_alignment.append(np.full(hp.order2npix(i), None))
-
-    # work forward - determine if we should map to a lower order pixel, this pixel, or keep looking.
-    for read_order in range(0, highest_order + 1):
-        parent_order = read_order - 1
-        for index in range(0, len(nested_sums[read_order])):
-            parent_alignment = None
-            if parent_order >= 0:
-                parent_pixel = index >> 2
-                parent_alignment = nested_alignment[parent_order][parent_pixel]
-
-            if parent_alignment:
-                nested_alignment[read_order][index] = parent_alignment
-            elif nested_sums[read_order][index] == 0:
-                continue
-            elif nested_sums[read_order][index] <= threshold:
-                nested_alignment[read_order][index] = (
-                    read_order,
-                    index,
-                    nested_sums[read_order][index],
-                )
-            elif read_order == highest_order:
-                raise ValueError(
-                    f"""single pixel count {
-                        nested_sums[read_order][index]} exceeds threshold {threshold}"""
-                )
-    return nested_alignment[highest_order]
+def pixel_is_polar(order, pix):
+    """Checks if a healpixel is a polar pixel.
 
-
-def generate_destination_pixel_map(histogram, pixel_map):
-    """Generate mapping from destination pixel to all the constituent pixels.
+    Args:
+        order (int): the healpix order of the pixel to be checked.
+        pix (int): the id of a healpixel to be checked. must be in the nested id scheme.
+    Returns:
+        tuple of a boolean and a string, the boolean indicating whether the pixel
+            polar and the string denoting which pole it is ('North' or 'South')).
+            string is empty in the case that the pixel isn't polar.
+    """
+    nside = hp.order2nside(order)
+    npix = hp.nside2npix(nside)
+    ring_pix = hp.nest2ring(nside, pix)
+
+    # in the ring numbering scheme, the first and last 4 pixels are the poles.
+    if ring_pix <= 3:
+        return (True, 'North')
+    if ring_pix >= npix - 4:
+        return (True, 'South')
+    return (False, '')
+
+def get_truncated_margin_pixels(order, pix, margin_order):
+    """Given a polar healpixel, find the margin pixels at order highest_k that will be
+    truncated at the poles. In other words, find the margin pixels that are also
+    polar pixels.
 
     Args:
-        histogram (:obj:`np.array`): one-dimensional numpy array of long integers where the
-            value at each index corresponds to the number of objects found at the healpix pixel.
-        pixel_map (:obj:`np.array`): one-dimensional numpy array of integer 3-tuples.
-            See :func:`generate_alignment` for more details on this format.
+        order (int): the healpix order of the pixel that we wish to
+            find the truncated margin pixels for. 
+        pix (int): the healpixel we wish to find the truncated margin pixels for.
+        margin_order (int): the healpixel order that our margin pixels are at. Must
+            be larger than `order`.
     Returns:
-        dictionary that maps the integer 3-tuple of a pixel at destination order to the set of
-        indexes in histogram for the pixels at the original healpix order
+        a list of margin pixels at margin_order order that will be truncated at 
+            the poles, i.e. the margin pixels that are also polar pixels 
+            themselves. In the case that pix is a polar pixel, it will return
+            3 pixels, otherwise it will return an empty list.
     """
-    # Find all distinct destination pixels
-    non_none_elements = pixel_map[pixel_map != np.array(None)]
-    unique_pixels = np.unique(non_none_elements)
-
-    # Compute the order from the number of pixels at the level.
-    max_order = hp.npix2order(len(histogram))
-
-    result = {}
-    for order, pixel, count in unique_pixels:
-        # Find all constituent pixels at the histogram's order
-        explosion_factor = 4 ** (max_order - int(order))
-        start_pixel = int(pixel) * explosion_factor
-        end_pixel = (int(pixel) + 1) * explosion_factor
+    if margin_order <= order:
+        raise ValueError("margin_order must be larger than order")
+
+    partition_nside = hp.order2nside(order)
+    margin_nside = hp.order2nside(margin_order)
+
+    polar, pole = pixel_is_polar(order, pix)
 
-        non_zero_indexes = np.nonzero(histogram[start_pixel:end_pixel])[0] + start_pixel
-        result[(order, pixel, count)] = non_zero_indexes.tolist()
+    if not polar:
+        return []
+
+    truncs = []
+
+    if pole == "North":
+        excluded_pixel = hp.nest2ring(partition_nside, pix)
+        for i in range(4):
+            if i != excluded_pixel:
+                truncs.append(hp.ring2nest(margin_nside, i))
+    else:
+        d_order = margin_order - order
+        excluded_pixel_nest = (4 ** d_order) * pix
+        excluded_pixel_ring = hp.nest2ring(margin_nside, excluded_pixel_nest)
+        npix = hp.nside2npix(margin_nside)
+
+        for j in range(npix - 4, npix):
+            if j != excluded_pixel_ring:
+                truncs.append(hp.ring2nest(margin_nside, j))
 
-    return result
+    return truncs
```

### Comparing `hipscat-0.0.8/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.0.9/src/hipscat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.0.8
+Version: 0.0.9
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Astronomy Data Commons
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-0.0.8/src/hipscat.egg-info/SOURCES.txt` & `hipscat-0.0.9/src/hipscat.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 src/hipscat/io/paths.py
 src/hipscat/io/write_metadata.py
 src/hipscat/io/file_io/__init__.py
 src/hipscat/io/file_io/file_io.py
 src/hipscat/io/file_io/file_pointer.py
 src/hipscat/pixel_math/README.md
 src/hipscat/pixel_math/__init__.py
+src/hipscat/pixel_math/healpix_pixel.py
 src/hipscat/pixel_math/hipscat_id.py
+src/hipscat/pixel_math/margin_bounding.py
 src/hipscat/pixel_math/partition_stats.py
 src/hipscat/pixel_math/pixel_margins.py
 tests/.pylintrc
 tests/conftest.py
 tests/data/small_sky/catalog_info.json
 tests/data/small_sky/partition_info.csv
 tests/data/small_sky/point_map.fits
@@ -67,10 +69,12 @@
 tests/hipscat/catalog/test_pixel_tree.py
 tests/hipscat/inspection/test_visualize_catalog.py
 tests/hipscat/io/conftest.py
 tests/hipscat/io/test_paths.py
 tests/hipscat/io/test_write_metadata.py
 tests/hipscat/io/file_io/test_file_io.py
 tests/hipscat/io/file_io/test_file_pointers.py
+tests/hipscat/pixel_math/test_healpix_pixel.py
 tests/hipscat/pixel_math/test_hipscat_id.py
+tests/hipscat/pixel_math/test_margin_bounding.py
 tests/hipscat/pixel_math/test_partition_stats.py
 tests/hipscat/pixel_math/test_pixel_margins.py
```

### Comparing `hipscat-0.0.8/tests/.pylintrc` & `hipscat-0.0.9/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/conftest.py` & `hipscat-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.0.9/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky/point_map.fits` & `hipscat-0.0.9/tests/data/small_sky/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.0.9/tests/data/small_sky_order1/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/catalog/conftest.py` & `hipscat-0.0.9/tests/hipscat/catalog/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/catalog/test_catalog.py` & `hipscat-0.0.9/tests/hipscat/catalog/test_catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Tests of catalog functionality"""
 
 import os
-import tempfile
 
 import pytest
 
 from hipscat.catalog import Catalog
 
 
 def test_load_catalog_small_sky(small_sky_dir):
@@ -20,44 +19,43 @@
     """Instantiate a catalog with 4 pixels"""
     cat = Catalog(small_sky_order1_dir)
 
     assert cat.catalog_name == "small_sky_order1"
     assert len(cat.get_pixels()) == 4
 
 
-def test_empty_directory():
+def test_empty_directory(tmp_path):
     """Test loading empty or incomplete data"""
-    with tempfile.TemporaryDirectory() as tmp_dir:
-        ## Path doesn't exist
-        with pytest.raises(FileNotFoundError):
-            Catalog(os.path.join("path", "empty"))
-
-        catalog_path = os.path.join(tmp_dir, "empty")
-        os.makedirs(catalog_path, exist_ok=True)
-
-        ## Path exists but there's nothing there
-        with pytest.raises(FileNotFoundError):
-            Catalog(catalog_path)
-
-        ## catalog_info file exists - getting closer
-        file_name = os.path.join(catalog_path, "catalog_info.json")
-        with open(
-            file_name,
-            "w",
-            encoding="utf-8",
-        ) as metadata_file:
-            metadata_file.write('{"catalog_name":"empty"}')
-
-        with pytest.raises(FileNotFoundError):
-            Catalog(catalog_path)
-
-        ## partition_info file exists - enough to create a catalog
-        file_name = os.path.join(catalog_path, "partition_info.csv")
-        with open(
-            file_name,
-            "w",
-            encoding="utf-8",
-        ) as metadata_file:
-            metadata_file.write("foo")
+    ## Path doesn't exist
+    with pytest.raises(FileNotFoundError):
+        Catalog(os.path.join("path", "empty"))
+
+    catalog_path = os.path.join(tmp_path, "empty")
+    os.makedirs(catalog_path, exist_ok=True)
+
+    ## Path exists but there's nothing there
+    with pytest.raises(FileNotFoundError):
+        Catalog(catalog_path)
+
+    ## catalog_info file exists - getting closer
+    file_name = os.path.join(catalog_path, "catalog_info.json")
+    with open(
+        file_name,
+        "w",
+        encoding="utf-8",
+    ) as metadata_file:
+        metadata_file.write('{"catalog_name":"empty"}')
+
+    with pytest.raises(FileNotFoundError):
+        Catalog(catalog_path)
+
+    ## partition_info file exists - enough to create a catalog
+    file_name = os.path.join(catalog_path, "partition_info.csv")
+    with open(
+        file_name,
+        "w",
+        encoding="utf-8",
+    ) as metadata_file:
+        metadata_file.write("foo")
 
-        catalog = Catalog(catalog_path)
-        assert catalog.catalog_name == "empty"
+    catalog = Catalog(catalog_path)
+    assert catalog.catalog_name == "empty"
```

### Comparing `hipscat-0.0.8/tests/hipscat/catalog/test_partition_info.py` & `hipscat-0.0.9/tests/hipscat/catalog/test_partition_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 """Tests of partition info functionality"""
 
 import os
 
 from hipscat.catalog import PartitionInfo
+from hipscat.pixel_math import HealpixPixel
 
 
 def test_load_partition_info_small_sky(small_sky_dir):
     """Instantiate the partition info for catalog with 1 pixel"""
     partitions = PartitionInfo(small_sky_dir)
 
     partition_file_list = partitions.get_file_names()
     assert len(partition_file_list) == 1
 
     for parquet_file in partition_file_list:
         assert os.path.exists(parquet_file)
 
+    order_pixel_pairs = partitions.get_healpix_pixels()
+    assert len(order_pixel_pairs) == 1
+    expected = [HealpixPixel(0, 11)]
+    assert order_pixel_pairs == expected
+
 
 def test_load_partition_info_small_sky_order1(small_sky_order1_dir):
     """Instantiate the partition info for catalog with 4 pixels"""
     partitions = PartitionInfo(small_sky_order1_dir)
 
     partition_file_list = partitions.get_file_names()
     assert len(partition_file_list) == 4
 
     for parquet_file in partition_file_list:
         assert os.path.exists(parquet_file)
+
+    order_pixel_pairs = partitions.get_healpix_pixels()
+    assert len(order_pixel_pairs) == 4
+    expected = [
+        HealpixPixel(1, 44),
+        HealpixPixel(1, 45),
+        HealpixPixel(1, 46),
+        HealpixPixel(1, 47),
+    ]
+    assert order_pixel_pairs == expected
```

### Comparing `hipscat-0.0.8/tests/hipscat/catalog/test_pixel_node.py` & `hipscat-0.0.9/tests/hipscat/catalog/test_pixel_node.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/catalog/test_pixel_tree.py` & `hipscat-0.0.9/tests/hipscat/catalog/test_pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.0.9/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/io/conftest.py` & `hipscat-0.0.9/tests/hipscat/io/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,16 @@
     return assert_text_file_matches
 
 
 @pytest.fixture
 def basic_catalog_info(tmp_path):
     return CatalogParameters(
         catalog_name="small_sky",
-        input_paths=["foo"],
-        input_format="csv",
         output_path=tmp_path,
-        highest_healpix_order=0,
-        ra_column="ra",
-        dec_column="dec",
+        total_rows=131,
     )
 
 
 @pytest.fixture
 def basic_catalog_parquet_metadata():
     return pa.schema(
         [
```

### Comparing `hipscat-0.0.8/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.0.9/tests/hipscat/io/file_io/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.0.9/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.8/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.0.9/tests/hipscat/io/test_write_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Tests of file IO (reads and writes)"""
 
 
 import os
 import shutil
 
-import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 import hipscat.io.file_io as file_io
 import hipscat.io.write_metadata as io
@@ -45,46 +44,39 @@
 
 
 def test_write_catalog_info(assert_text_file_matches, tmp_path, basic_catalog_info):
     """Test that we accurately write out catalog metadata"""
     expected_lines = [
         "{",
         '    "catalog_name": "small_sky",',
-        r'    "version": ".*",',  # version matches digits
-        r'    "generation_date": "[.\d]+",',  # date matches date format
+        '    "catalog_type": "object",',
         '    "epoch": "J2000",',
         '    "ra_kw": "ra",',
         '    "dec_kw": "dec",',
-        '    "id_kw": "id",',
-        '    "total_objects": 131,',
-        '    "origin_healpix_order": 0',
-        '    "pixel_threshold": 1000000',
+        '    "total_rows": 131',
         "}",
     ]
 
-    initial_histogram = np.asarray([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 131])
-
-    io.write_catalog_info(basic_catalog_info, initial_histogram)
+    io.write_catalog_info(basic_catalog_info)
     metadata_filename = os.path.join(tmp_path, "small_sky", "catalog_info.json")
     assert_text_file_matches(expected_lines, metadata_filename)
 
 
 def test_write_provenance_info(assert_text_file_matches, tmp_path, basic_catalog_info):
     """Test that we accurately write out tool-provided generation metadata"""
     expected_lines = [
         "{",
         '    "catalog_name": "small_sky",',
+        '    "catalog_type": "object",',
         r'    "version": ".*",',  # version matches digits
         r'    "generation_date": "[.\d]+",',  # date matches date format
         '    "epoch": "J2000",',
         '    "ra_kw": "ra",',
         '    "dec_kw": "dec",',
-        '    "id_kw": "id",',
-        '    "origin_healpix_order": 0',
-        '    "pixel_threshold": 1000000',
+        '    "total_rows": 131,',
         '    "tool_args": {',
         '        "tool_name": "hipscat-import",',
         '        "tool_version": "1.0.0",',
         r'        "input_file_names": \[',
         '            "file1",',
         '            "file2",',
         '            "file3"',
@@ -144,74 +136,41 @@
     ]
     pixel_map = {tuple([0.0, 11.0, 131.0]): [44.0, 45.0, 46.0]}
     io.write_partition_info(basic_catalog_info, pixel_map)
     metadata_filename = os.path.join(tmp_path, "small_sky", "partition_info.csv")
     assert_text_file_matches(expected_lines, metadata_filename)
 
 
-def test_write_legacy_metadata_file(
-    assert_text_file_matches, tmp_path, basic_catalog_info
-):
-    """Test that we can write out the older version of the partition metadata"""
-    expected_lines = [
-        "{",
-        '    "cat_name": "small_sky",',
-        '    "ra_kw": "ra",',
-        '    "dec_kw": "dec",',
-        '    "id_kw": "id",',
-        '    "n_sources": 131,',
-        '    "pix_threshold": 1000000,',
-        r'    "urls": \[',
-        '        "foo"',
-        "    ],",
-        '    "hips": {',
-        r'        "0": \[',
-        "            11",
-        "        ]",
-        "    }",
-        "}",
-    ]
-    initial_histogram = np.asarray([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 131])
-    pixel_map = np.full(12, None)
-    pixel_map[11] = (0, 11, 131)
-
-    io.write_legacy_metadata(basic_catalog_info, initial_histogram, pixel_map)
-
-    metadata_filename = os.path.join(tmp_path, "small_sky", "small_sky_meta.json")
-
-    assert_text_file_matches(expected_lines, metadata_filename)
-
-
 def test_write_parquet_metadata(
     tmp_path, small_sky_dir, basic_catalog_parquet_metadata
 ):
     """Copy existing catalog and create new metadata files for it"""
     temp_path = os.path.join(tmp_path, "catalog")
     shutil.copytree(
         small_sky_dir,
         temp_path,
     )
     io.write_parquet_metadata(temp_path)
     check_parquet_schema(
-        os.path.join(tmp_path, "catalog", "_metadata"), basic_catalog_parquet_metadata
+        os.path.join(temp_path, "_metadata"), basic_catalog_parquet_metadata
     )
     ## _common_metadata has 0 row groups
     check_parquet_schema(
-        os.path.join(tmp_path, "catalog", "_common_metadata"),
+        os.path.join(temp_path, "_common_metadata"),
         basic_catalog_parquet_metadata,
         0,
     )
     ## Re-write - should still have the same properties.
     io.write_parquet_metadata(temp_path)
     check_parquet_schema(
-        os.path.join(tmp_path, "catalog", "_metadata"), basic_catalog_parquet_metadata
+        os.path.join(temp_path, "_metadata"), basic_catalog_parquet_metadata
     )
     ## _common_metadata has 0 row groups
     check_parquet_schema(
-        os.path.join(tmp_path, "catalog", "_common_metadata"),
+        os.path.join(temp_path, "_common_metadata"),
         basic_catalog_parquet_metadata,
         0,
     )
 
 
 def test_write_parquet_metadata_order1(
     tmp_path, small_sky_order1_dir, basic_catalog_parquet_metadata
@@ -223,21 +182,21 @@
         small_sky_order1_dir,
         temp_path,
     )
 
     io.write_parquet_metadata(temp_path)
     ## 4 row groups for 4 partitioned parquet files
     check_parquet_schema(
-        os.path.join(tmp_path, "catalog", "_metadata"),
+        os.path.join(temp_path, "_metadata"),
         basic_catalog_parquet_metadata,
         4,
     )
     ## _common_metadata has 0 row groups
     check_parquet_schema(
-        os.path.join(tmp_path, "catalog", "_common_metadata"),
+        os.path.join(temp_path, "_common_metadata"),
         basic_catalog_parquet_metadata,
         0,
     )
 
 
 def test_write_index_parquet_metadata(tmp_path):
     """Create an index-like catalog, and test metadata creation."""
@@ -281,14 +240,21 @@
     npt.assert_array_equal(schema.names, expected_schema.names)
 
     assert schema.equals(expected_schema, check_metadata=False)
 
     parquet_file = pq.ParquetFile(file_name)
     assert parquet_file.metadata.num_row_groups == expected_num_row_groups
 
+    for row_index in range(0, parquet_file.metadata.num_row_groups):
+        row_md = parquet_file.metadata.row_group(row_index)
+        for column_index in range(0, row_md.num_columns):
+            column_metadata = row_md.column(column_index)
+            assert column_metadata.file_path.endswith(".parquet")
+
+
 
 def test_read_write_fits_point_map(tmp_path):
     """Check that we write and can read a FITS file for spatial distribution."""
     initial_histogram = hist.empty_histogram(1)
     filled_pixels = [51, 29, 51, 0]
     initial_histogram[44:] = filled_pixels[:]
     io.write_fits_map(tmp_path, initial_histogram)
```

### Comparing `hipscat-0.0.8/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.0.9/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files identical despite different names*

