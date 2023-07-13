# Comparing `tmp/curated-transformers-0.1.1.tar.gz` & `tmp/curated-transformers-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-0.1.1.tar", last modified: Wed May 24 07:10:38 2023, max compression
+gzip compressed data, was "curated-transformers-1.0.0.dev0.tar", last modified: Thu Jul 13 11:29:37 2023, max compression
```

## Comparing `curated-transformers-0.1.1.tar` & `curated-transformers-1.0.0.dev0.tar`

### file list

```diff
@@ -1,60 +1,196 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)      933 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      620 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.767744 curated-transformers-0.1.1/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      313 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/_compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.767744 curated-transformers-0.1.1/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/activations.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2362 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2258 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/attention.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1738 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4774 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/curated_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10980 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/hf_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1556 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1780 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1881 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/scalar_weight.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1254 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)       94 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/albert/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2969 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1441 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/test_torchscript.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tokenization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.767744 curated-transformers-0.1.1/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      933 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)      589 2023-05-24 07:10:38.775744 curated-transformers-0.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      116 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     4290 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3972 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.537990 curated-transformers-1.0.0.dev0/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/generation/
+-rw-r--r--   0 vsts      (1001) docker     (122)      261 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2508 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3268 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3410 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/default_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1917 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4281 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      791 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/generator_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1183 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3298 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/logits.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4992 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/state.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2794 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/stop_conditions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2111 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/string_generator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1468 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/activations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17092 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/attention.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1407 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10491 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3867 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/feedforward.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1511 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2514 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/scalar_weight.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      360 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3660 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4109 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3249 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1734 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4792 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/auto_model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3497 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6957 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3561 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2619 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2852 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/layer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      681 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3579 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2803 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6335 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3420 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3874 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/layer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      157 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2834 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6950 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3997 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/layer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4460 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (122)      140 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2823 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6528 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3893 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/layer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4482 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/module.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4764 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3302 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2155 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2684 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       33 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      682 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      126 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2505 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5982 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/impl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1101 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      677 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/quantizable.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3002 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      847 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4647 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4514 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4539 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_generic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2522 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_logits.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2860 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_stop.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      703 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/bert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2550 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1378 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3916 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1367 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3917 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      511 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/roberta/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3789 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2008 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_auto_models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3415 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1324 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3732 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/test_generation.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10744 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10642 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      733 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10778 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      977 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3909 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30593 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2924 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/_hf_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3523 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2661 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3021 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)      385 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2325 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/_fairseq.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11948 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4435 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7336 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2781 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4092 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2250 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3230 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3885 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11770 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      221 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/curated_transformers/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1208 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/pytorch.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7392 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/serde.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.537990 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4290 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     7667 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       93 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)      702 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/setup.py
```

### Comparing `curated-transformers-0.1.1/LICENSE` & `curated-transformers-1.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.1/curated_transformers/models/bert/encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/encoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,87 @@
-from typing import Optional
+from typing import Any, Mapping, Optional, Type, TypeVar
 
 import torch
-from torch.nn import Module
 from torch import Tensor
 
-from .config import BertConfig
-from .embeddings import BertEmbeddings
-from .layer import BertEncoderLayer
-from ..attention import AttentionMask
-from ..output import PyTorchTransformerOutput
+from ...layers.attention import AttentionMask
+from ..bert.layer import BERTEncoderLayer
+from ..hf_hub import FromHFHub
+from ..module import EncoderModule
+from ..output import ModelOutput
+from ._hf import convert_hf_config, convert_hf_state_dict
+from .config import RoBERTaConfig
+from .embeddings import RoBERTaEmbeddings
+
+# Only provided as typing.Self in Python 3.11+.
+Self = TypeVar("Self", bound="RoBERTaEncoder")
+
+
+class RoBERTaEncoder(EncoderModule, FromHFHub):
+    """
+    RoBERTa (`Liu et al., 2019`_) encoder.
 
+    .. _Liu et al., 2019: https://arxiv.org/abs/1907.11692
+    """
 
-class BertEncoder(Module):
-    def __init__(
-        self,
-        config: BertConfig,
-    ):
+    def __init__(self, config: RoBERTaConfig, *, device: Optional[torch.device] = None):
+        """
+        Construct a RoBERTa encoder.
+
+        :param config:
+            Encoder configuration.
+        :param device:
+            Device to which the module is to be moved.
+        :returns:
+            The encoder.
+        """
         super().__init__()
 
-        self.embeddings = BertEmbeddings(config.embedding, config.layer)
-        self.padding_idx = config.padding_idx
+        self.embeddings = RoBERTaEmbeddings(
+            config.embedding, config.layer, padding_id=config.padding_id, device=device
+        )
+        self.padding_id = config.padding_id
         self.max_seq_len = config.model_max_length
         self.layers = torch.nn.ModuleList(
             [
-                BertEncoderLayer(config.layer, config.attention)
+                BERTEncoderLayer(config.layer, config.attention, device=device)
                 for _ in range(config.layer.num_hidden_layers)
             ]
         )
 
     def _create_attention_mask(self, x: Tensor) -> AttentionMask:
-        return AttentionMask(bool_mask=x.ne(self.padding_idx))
+        return AttentionMask(x.ne(self.padding_id))
 
     def forward(
         self,
         input_ids: Tensor,
         attention_mask: Optional[AttentionMask] = None,
         token_type_ids: Optional[Tensor] = None,
-    ) -> PyTorchTransformerOutput:
-        """
-        Shapes:
-            input_ids, attention_mask, token_type_ids - (batch, seq_len)
-        """
+    ) -> ModelOutput:
         if attention_mask is None:
             attention_mask = self._create_attention_mask(input_ids)
 
         embeddings = self.embeddings(input_ids, token_type_ids, None)
         layer_output = embeddings
 
         layer_outputs = []
         for layer in self.layers:
             layer_output = layer(layer_output, attention_mask)
             layer_outputs.append(layer_output)
 
-        return PyTorchTransformerOutput(
+        return ModelOutput(
             embedding_output=embeddings, layer_hidden_states=layer_outputs
         )
+
+    @classmethod
+    def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
+        return convert_hf_state_dict(params)
+
+    @classmethod
+    def from_hf_config(
+        cls: Type[Self],
+        *,
+        hf_config: Any,
+        device: Optional[torch.device] = None,
+    ) -> Self:
+        config = convert_hf_config(hf_config)
+        return cls(config, device=device)
```

### Comparing `curated-transformers-0.1.1/setup.cfg` & `curated-transformers-1.0.0.dev0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [metadata]
-version = 0.1.1
+version = 1.0.0.dev0
 description = Curated transformer models
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = true
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
+	curated-tokenizers>=0.9.0.dev0,<1.0.0
+	huggingface-hub>=0.14
+	tokenizers>=0.13.3
 	torch>=1.12.0
 
 [bdist_wheel]
 universal = true
 
 [sdist]
 formats = gztar
 
 [mypy]
 exclude = tests
+allow_redefinition = True
 ignore_missing_imports = True
 no_implicit_optional = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

