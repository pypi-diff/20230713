# Comparing `tmp/gbd_mapping-3.1.0.tar.gz` & `tmp/gbd_mapping-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_mapping-3.1.0.tar", last modified: Thu Jun  1 23:20:50 2023, max compression
+gzip compressed data, was "gbd_mapping-3.1.1.tar", last modified: Thu Jul 13 20:33:38 2023, max compression
```

## Comparing `gbd_mapping-3.1.0.tar` & `gbd_mapping-3.1.1.tar`

### file list

```diff
@@ -1,62 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.234713 gbd_mapping-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.238713 gbd_mapping-3.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.238713 gbd_mapping-3.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/gbd_mapping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/gbd_mapping_generator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.234713 gbd_mapping-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.242713 gbd_mapping-3.1.0/src/gbd_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/base_template.py
--rw-r--r--   0 runner    (1001) docker     (123)   421863 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/cause.py
--rw-r--r--   0 runner    (1001) docker     (123)    42887 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/cause_template.py
--rw-r--r--   0 runner    (1001) docker     (123)   403799 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)   282616 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/covariate_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/etiology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/etiology_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/id.py
--rw-r--r--   0 runner    (1001) docker     (123)   223458 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/risk_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/risk_factor_template.py
--rw-r--r--   0 runner    (1001) docker     (123)   761067 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/sequela.py
--rw-r--r--   0 runner    (1001) docker     (123)   441749 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/sequela_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.242713 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/src/gbd_mapping_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/base_template_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/build_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/cause_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/covariate_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/etiology_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/id_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/risk_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/sequela_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/tests/test_gbd_mapping_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.432549 gbd_mapping-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.424549 gbd_mapping-3.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.424549 gbd_mapping-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-13 20:33:38.432549 gbd_mapping-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.424549 gbd_mapping-3.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.424549 gbd_mapping-3.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.424549 gbd_mapping-3.1.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/source/gbd_mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/source/gbd_mapping_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:33:38.432549 gbd_mapping-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.424549 gbd_mapping-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.428549 gbd_mapping-3.1.1/src/gbd_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)   421863 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42887 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/cause_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)   403799 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   282616 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/covariate_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/etiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/etiology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223458 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/risk_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/risk_factor_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)   761067 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/sequela.py
+-rw-r--r--   0 runner    (1001) docker     (123)   441749 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping/sequela_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.428549 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 20:33:38.000000 gbd_mapping-3.1.1/src/gbd_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.432549 gbd_mapping-3.1.1/src/gbd_mapping_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/base_template_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/build_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/cause_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/covariate_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/etiology_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/id_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/risk_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/sequela_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/src/gbd_mapping_generator/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:38.432549 gbd_mapping-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/tests/test_gbd_mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 20:33:27.000000 gbd_mapping-3.1.1/tox.ini
```

### Comparing `gbd_mapping-3.1.0/CHANGELOG.rst` & `gbd_mapping-3.1.1/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+**3.1.1 - 07/13/23**
+
+ - Changes version metadata to use setuptools_scm
+
+
 **3.1.0 - 06/01/23**
 
  - Update vivarium_gbd_access pin 
  - Support Python 3.8-3.11 
  - Update git actions to remove warnings
 
 **3.0.6 - 07/05/22**
```

### Comparing `gbd_mapping-3.1.0/CODE_OF_CONDUCT.rst` & `gbd_mapping-3.1.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/CONTRIBUTING.rst` & `gbd_mapping-3.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/LICENSE.txt` & `gbd_mapping-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/PKG-INFO` & `gbd_mapping-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_mapping
-Version: 3.1.0
+Version: 3.1.1
 Summary: A programmatically accessible mapping of gbd entities.
 Home-page: https://github.com/ihmeuw/gbd_mapping
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
```

### Comparing `gbd_mapping-3.1.0/README.rst` & `gbd_mapping-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/docs/Makefile` & `gbd_mapping-3.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/docs/source/conf.py` & `gbd_mapping-3.1.1/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     exec(f.read(), about)
 
 sys.path.insert(0, str(Path("..").resolve()))
 
 # -- Project information -----------------------------------------------------
 
 project = about["__title__"]
-copyright = f'2022, {about["__author__"]}'
+copyright = f'2023, {about["__author__"]}'
 author = about["__author__"]
 
 # The short X.Y version.
-version = about["__version__"]
+version = gbd_mapping.__version__
 # The full version, including alpha/beta/rc tags.
-release = about["__version__"]
+release = gbd_mapping.__version__
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 
 needs_sphinx = "4.0"
```

### Comparing `gbd_mapping-3.1.0/docs/source/gbd_mapping.rst` & `gbd_mapping-3.1.1/docs/source/gbd_mapping.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/docs/source/gbd_mapping_generator.rst` & `gbd_mapping-3.1.1/docs/source/gbd_mapping_generator.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/setup.py` & `gbd_mapping-3.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 import os
 
 from setuptools import find_packages, setup
 
 if __name__ == "__main__":
-
     base_dir = os.path.dirname(__file__)
     src_dir = os.path.join(base_dir, "src")
 
     about = {}
     with open(os.path.join(src_dir, "gbd_mapping", "__about__.py")) as f:
         exec(f.read(), about)
 
@@ -18,14 +17,16 @@
     install_requirements = [
         "click",
         "numpy",
         "pandas",
         "pyyaml",
     ]
 
+    setup_requires = ["setuptools_scm"]
+
     data_requires = [
         "vivarium-gbd-access>=3.0.7",
     ]
 
     test_requirements = [
         "pytest",
         "pytest-mock",
@@ -34,15 +35,14 @@
     doc_requirements = [
         "sphinx",
         "sphinx-rtd-theme",
     ]
 
     setup(
         name=about["__title__"],
-        version=about["__version__"],
         description=about["__summary__"],
         long_description=long_description,
         url=about["__uri__"],
         author=about["__author__"],
         author_email=about["__email__"],
         package_dir={"": "src"},
         packages=find_packages(where="src"),
@@ -56,8 +56,14 @@
             "dev": doc_requirements + test_requirements + data_requires,
         },
         entry_points="""
                 [console_scripts]
                 build_mapping=gbd_mapping_generator.build_mapping:build_mapping
             """,
         zip_safe=False,
+        use_scm_version={
+            "write_to": "src/gbd_mapping/_version.py",
+            "write_to_template": '__version__ = "{version}"\n',
+            "tag_regex": r"^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$",
+        },
+        setup_requires=setup_requires,
     )
```

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/base_template.py` & `gbd_mapping-3.1.1/src/gbd_mapping/base_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/cause.py` & `gbd_mapping-3.1.1/src/gbd_mapping/cause.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/cause_template.py` & `gbd_mapping-3.1.1/src/gbd_mapping/cause_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/covariate.py` & `gbd_mapping-3.1.1/src/gbd_mapping/covariate.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/covariate_template.py` & `gbd_mapping-3.1.1/src/gbd_mapping/covariate_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/etiology.py` & `gbd_mapping-3.1.1/src/gbd_mapping/etiology.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/etiology_template.py` & `gbd_mapping-3.1.1/src/gbd_mapping/etiology_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/id.py` & `gbd_mapping-3.1.1/src/gbd_mapping/id.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/risk_factor.py` & `gbd_mapping-3.1.1/src/gbd_mapping/risk_factor.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/risk_factor_template.py` & `gbd_mapping-3.1.1/src/gbd_mapping/risk_factor_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/sequela.py` & `gbd_mapping-3.1.1/src/gbd_mapping/sequela.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping/sequela_template.py` & `gbd_mapping-3.1.1/src/gbd_mapping/sequela_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping.egg-info/PKG-INFO` & `gbd_mapping-3.1.1/src/gbd_mapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-mapping
-Version: 3.1.0
+Version: 3.1.1
 Summary: A programmatically accessible mapping of gbd entities.
 Home-page: https://github.com/ihmeuw/gbd_mapping
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
```

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping.egg-info/SOURCES.txt` & `gbd_mapping-3.1.1/src/gbd_mapping.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
+.gitattributes
+.gitignore
+.readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
+tox.ini
+.github/CODEOWNERS
+.github/pull_request_template.md
+.github/workflows/build.yml
+.github/workflows/deploy.yml
 docs/Makefile
 docs/nitpick-exceptions
 docs/source/conf.py
 docs/source/gbd_mapping.rst
 docs/source/gbd_mapping_generator.rst
 docs/source/index.rst
 docs/source/modules.rst
 docs/source/_static/style.css
 src/gbd_mapping/__about__.py
 src/gbd_mapping/__init__.py
+src/gbd_mapping/_version.py
 src/gbd_mapping/base_template.py
 src/gbd_mapping/cause.py
 src/gbd_mapping/cause_template.py
 src/gbd_mapping/covariate.py
 src/gbd_mapping/covariate_template.py
 src/gbd_mapping/etiology.py
 src/gbd_mapping/etiology_template.py
```

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/base_template_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/base_template_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/build_mapping.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/build_mapping.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/cause_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/cause_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/covariate_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/covariate_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/data.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/data.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/etiology_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/etiology_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/id_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/id_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/risk_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/risk_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/sequela_builder.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/sequela_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.1.0/src/gbd_mapping_generator/util.py` & `gbd_mapping-3.1.1/src/gbd_mapping_generator/util.py`

 * *Files identical despite different names*

