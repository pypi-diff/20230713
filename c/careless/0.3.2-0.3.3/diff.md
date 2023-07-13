# Comparing `tmp/careless-0.3.2.tar.gz` & `tmp/careless-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.3.2.tar", last modified: Mon Jul  3 15:35:51 2023, max compression
+gzip compressed data, was "careless-0.3.3.tar", last modified: Thu Jul 13 21:22:53 2023, max compression
```

## Comparing `careless-0.3.2.tar` & `careless-0.3.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 15:35:37.000000 careless-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 15:35:37.000000 careless-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-03 15:35:51.123209 careless-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-03 15:35:37.000000 careless-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.115202 careless-0.3.2/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 15:35:37.000000 careless-0.3.2/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 15:35:37.000000 careless-0.3.2/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 15:35:37.000000 careless-0.3.2/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4879 2023-07-03 15:35:37.000000 careless-0.3.2/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/xds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-03 15:35:37.000000 careless-0.3.2/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/prior_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.115202 careless-0.3.2/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-03 15:35:51.000000 careless-0.3.2/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-03 15:35:37.000000 careless-0.3.2/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-03 15:35:37.000000 careless-0.3.2/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 15:35:51.123209 careless-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-03 15:35:37.000000 careless-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-03 15:35:37.000000 careless-0.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-03 15:35:37.000000 careless-0.3.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 21:22:42.000000 careless-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 21:22:42.000000 careless-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 21:22:53.940818 careless-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-13 21:22:42.000000 careless-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.932819 careless-0.3.3/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 21:22:42.000000 careless-0.3.3/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-13 21:22:42.000000 careless-0.3.3/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-13 21:22:42.000000 careless-0.3.3/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-07-13 21:22:42.000000 careless-0.3.3/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-13 21:22:42.000000 careless-0.3.3/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/prior_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.932819 careless-0.3.3/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-13 21:22:42.000000 careless-0.3.3/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-13 21:22:42.000000 careless-0.3.3/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 21:22:53.940818 careless-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-13 21:22:42.000000 careless-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-13 21:22:42.000000 careless-0.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-13 21:22:42.000000 careless-0.3.3/tests/test_cli.py
```

### Comparing `careless-0.3.2/LICENSE` & `careless-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/PKG-INFO` & `careless-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.2
+Version: 0.3.3
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.2/README.md` & `careless-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/common.py` & `careless-0.3.3/careless/args/common.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/crossvalidation.py` & `careless-0.3.3/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/filtration.py` & `careless-0.3.3/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/interpretation.py` & `careless-0.3.3/careless/args/interpretation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/optimizer.py` & `careless-0.3.3/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/poly.py` & `careless-0.3.3/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/positional_encoding.py` & `careless-0.3.3/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/prior.py` & `careless-0.3.3/careless/args/prior.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/required.py` & `careless-0.3.3/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/scaling.py` & `careless-0.3.3/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/args/tf_options.py` & `careless-0.3.3/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/callbacks/progress_bar.py` & `careless-0.3.3/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/careless.py` & `careless-0.3.3/careless/careless.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,29 +71,24 @@
     import pickle
     with open(parser.output_base + "_data_manager.pickle", "wb") as out:
         pickle.dump(dm, out)
 
     predictions_data = None
     if test is not None:
         for file_id, (ds_train, ds_test) in enumerate(zip(
-                dm.get_predictions(model, train),
-                dm.get_predictions(model, test),
+                dm.get_predictions(model, train, test_value=0),
+                dm.get_predictions(model, test, test_value=1),
                 )):
-            ds_train['test'] = rs.DataSeries(0, index=ds_train.index, dtype='I')
-            ds_test['test']  = rs.DataSeries(1, index=ds_test.index, dtype='I')
-
             filename = parser.output_base + f'_predictions_{file_id}.mtz'
             rs.concat((
                 ds_train,
                 ds_test,
             )).write_mtz(filename)
     else:
-        for file_id, ds_train in enumerate(dm.get_predictions(model, train)):
-            ds_train['test'] = rs.DataSeries(0, index=ds_train.index, dtype='I')
-
+        for file_id, ds_train in enumerate(dm.get_predictions(model, train, test_value=0)):
             filename = parser.output_base + f'_predictions_{file_id}.mtz'
             ds_train.write_mtz(filename)
 
     if parser.merge_half_datasets:
         scaling_model = model.scaling_model
         scaling_model.trainable = False
         xval_data = [None] * len(dm.asu_collection)
```

### Comparing `careless-0.3.2/careless/io/asu.py` & `careless-0.3.3/careless/io/asu.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/io/formatter.py` & `careless-0.3.3/careless/io/formatter.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/io/manager.py` & `careless-0.3.3/careless/io/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,64 +80,86 @@
         inputs = tuple(inputs)
         iobs = BaseModel.get_intensities(inputs)
         sigiobs = BaseModel.get_uncertainties(inputs)
         packed  = (inputs, iobs, sigiobs)
         tfds = tf.data.Dataset.from_tensor_slices(packed)
         return tfds.batch(len(iobs))
 
-    def get_predictions(self, model, inputs=None):
+    def get_predictions(self, model, inputs=None, test_value=0):
         """ 
         Extract results from a surrogate_posterior.
 
         Parameters
         ----------
         model : VariationalMergingModel
             A merging model from careless
         inputs : tuple (optional)
             Inputs for which to make the predictions if None, self.inputs is used.
+        test_value : int (optional)
+            Optionally change the value of the `test` column used for crossvalidation.
+            The default is 0. 
 
         Returns
         -------
         predictions : tuple
             A tuple of rs.DataSet objects containing the predictions for each 
             ReciprocalASU contained in self.asu_collection
         """
+        laue = BaseModel.is_laue(inputs)
+
         if inputs is None:
             inputs = self.inputs
 
         refl_id = BaseModel.get_refl_id(inputs)
+        asu_id,H = self.asu_collection.to_asu_id_and_miller_index(refl_id)
+        asu_id = asu_id.flatten()
+        file_id = model.get_file_id(inputs).flatten()
+        image_id = model.get_image_id(inputs).flatten()
+        if laue:
+            harmonic_id = BaseModel.get_harmonic_id(inputs).flatten()
+        else:
+            harmonic_id = np.arange(len(refl_id))
+        h,k,l = H.T
+
+        output = rs.DataSet({
+            'H' : rs.DataSeries(h, dtype='H'),
+            'K' : rs.DataSeries(k, dtype='H'),
+            'L' : rs.DataSeries(l, dtype='H'),
+            'harmonic_id' : rs.DataSeries(harmonic_id, dtype='I'),
+            'asu_id'      : rs.DataSeries(asu_id, dtype='I'),
+            'image_id'    : rs.DataSeries(image_id, dtype='I'),
+            'file_id'     : rs.DataSeries(file_id, dtype='I'),
+            'test'        : rs.DataSeries(test_value * np.ones_like(h), dtype='I'),
+        }, merged=False).groupby('harmonic_id').first().reset_index()
+        del(output['harmonic_id'])
+
         iobs = BaseModel.get_intensities(inputs).flatten()
         sig_iobs = BaseModel.get_uncertainties(inputs).flatten()
-        asu_id,H = self.asu_collection.to_asu_id_and_miller_index(refl_id)
-        #ipred = model(inputs)
         ipred,sigipred = model.prediction_mean_stddev(inputs)
         scale,sigscale = model.scale_mean_stddev(inputs)
 
-        h,k,l = H.T
-        results = ()
-        for i,asu in enumerate(self.asu_collection):
-            idx = asu_id == i
-            idx = idx.flatten()
-            output = rs.DataSet({
-                'H' : h[idx],
-                'K' : k[idx],
-                'L' : l[idx],
-                'Iobs' : iobs[idx],
-                'SigIobs' : sig_iobs[idx],
-                'Ipred' : ipred[idx],
-                'SigIpred' : sigipred[idx],
-                'Scale' : scale[idx],
-                'SigScale' : sigscale[idx],
-                }, 
-                cell=asu.cell, 
-                spacegroup=asu.spacegroup,
-                merged=False,
-            ).infer_mtz_dtypes().set_index(['H', 'K', 'L'])
-            results += (output, )
-        return results
+        num_refls = len(output)
+        data_cols = {
+            'Iobs'    : rs.DataSeries(iobs[:num_refls], dtype='J'),
+            'SigIobs' : rs.DataSeries(sig_iobs[:num_refls], dtype='Q'),
+            'Ipred'   : rs.DataSeries(ipred[:num_refls], dtype='J'),
+            'SigIpred': rs.DataSeries(sigipred[:num_refls], dtype='Q'),
+            'Scale'   : rs.DataSeries(scale[:num_refls], dtype='J'),
+            'SigScale': rs.DataSeries(sigscale[:num_refls], dtype='Q'),
+        }
+        for k,v in data_cols.items():
+            output[k] = v
+
+        for i,rasu in enumerate(self.asu_collection):
+            idx = output['asu_id'] == i
+            result = output.loc[idx]
+            result.cell = rasu.cell
+            result.spacegroup = rasu.spacegroup
+            yield result.set_index(['H', 'K', 'L'])
+
 
     def get_results(self, surrogate_posterior, inputs=None, output_parameters=True, max_intensity_snr=1e-5):
         """ 
         Extract results from a surrogate_posterior.
 
         Parameters
         ----------
```

### Comparing `careless-0.3.2/careless/io/xds.py` & `careless-0.3.3/careless/io/xds.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/base.py` & `careless-0.3.3/careless/models/base.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/likelihoods/laue.py` & `careless-0.3.3/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/likelihoods/mono.py` & `careless-0.3.3/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.3/careless/models/merging/surrogate_posteriors.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/merging/variational.py` & `careless-0.3.3/careless/models/merging/variational.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/priors/empirical.py` & `careless-0.3.3/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/priors/wilson.py` & `careless-0.3.3/careless/models/priors/wilson.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/scaling/image.py` & `careless-0.3.3/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/models/scaling/nn.py` & `careless-0.3.3/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/parser.py` & `careless-0.3.3/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/ccanom.py` & `careless-0.3.3/careless/stats/ccanom.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/cchalf.py` & `careless-0.3.3/careless/stats/cchalf.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/ccpred.py` & `careless-0.3.3/careless/stats/ccpred.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/completeness.py` & `careless-0.3.3/careless/stats/completeness.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/parser.py` & `careless-0.3.3/careless/stats/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/prior_b.py` & `careless-0.3.3/careless/stats/prior_b.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/rescale.py` & `careless-0.3.3/careless/stats/rescale.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/stats/rsplit.py` & `careless-0.3.3/careless/stats/rsplit.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/utils/distributions.py` & `careless-0.3.3/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/utils/laue.py` & `careless-0.3.3/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless/utils/positional_encoding.py` & `careless-0.3.3/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/careless.egg-info/PKG-INFO` & `careless-0.3.3/careless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.2
+Version: 0.3.3
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.2/careless.egg-info/SOURCES.txt` & `careless-0.3.3/careless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/scripts/make_difference_map` & `careless-0.3.3/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/scripts/stream2mtz` & `careless-0.3.3/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/setup.py` & `careless-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.2/tests/conftest.py` & `careless-0.3.3/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 import pytest
-from os import listdir
-from os.path import dirname, abspath, join
+from os import listdir,mkdir
+from os.path import dirname, abspath, join, exists
 import numpy as np
 import pandas as pd
 import re
 import reciprocalspaceship as rs
 import gemmi
 
+def pytest_sessionstart(session):
+    rundir = "data/"
+    rundir = abspath(join(dirname(__file__), rundir))
+
+    command = """
+    careless poly 
+        --disable-progress-bar 
+        --iterations=10 
+        --merge-half-datasets 
+        --half-dataset-repeats=3 
+        --test-fraction=0.1 
+        --disable-gpu 
+        --anomalous 
+        --wavelength-key=Wavelength
+        dHKL,Hobs,Kobs,Lobs,Wavelength
+        pyp_off.mtz 
+        pyp_2ms.mtz 
+        output/pyp
+    """
+    if not exists(f"{rundir}/output"):
+        mkdir(f"{rundir}/output")
+        from subprocess import call
+        call(command.split(), cwd=rundir)
+
 @pytest.fixture
 def cell_and_spacegroups():
     data = [
         ((10., 20., 30., 90., 80., 75.), 'P 1'),
         ((30., 50., 80., 90., 100., 90.), 'P 1 21 1'),    
         ((10., 20., 30., 90., 90., 90.), 'P 21 21 21'),
         ((89., 89., 105., 90., 90., 120.), 'P 31 2 1'),
```

### Comparing `careless-0.3.2/tests/test_cli.py` & `careless-0.3.3/tests/test_cli.py`

 * *Files identical despite different names*

