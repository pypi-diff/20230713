# Comparing `tmp/curated-transformers-0.9.0.tar.gz` & `tmp/curated-transformers-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-0.9.0.tar", last modified: Thu Jul 13 12:58:37 2023, max compression
+gzip compressed data, was "curated-transformers-1.0.0.dev0.tar", last modified: Thu Jul 13 11:29:37 2023, max compression
```

## Comparing `curated-transformers-0.9.0.tar` & `curated-transformers-1.0.0.dev0.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.029990 curated-transformers-0.9.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      116 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     4313 2023-07-13 12:58:37.029990 curated-transformers-0.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3972 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.009990 curated-transformers-0.9.0/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.013990 curated-transformers-0.9.0/curated_transformers/generation/
--rw-r--r--   0 vsts      (1001) docker     (122)      261 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2508 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3268 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3410 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/default_generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1917 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4281 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)      791 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/generator_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1183 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3298 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/logits.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4992 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/state.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2794 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/stop_conditions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2111 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/generation/string_generator.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.013990 curated-transformers-0.9.0/curated_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1468 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/activations.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17092 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/attention.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1407 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10491 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3867 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/feedforward.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1511 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/normalization.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2514 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/layers/scalar_weight.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.013990 curated-transformers-0.9.0/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      360 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.013990 curated-transformers-0.9.0/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3660 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/albert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4109 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3249 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1734 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4792 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/auto_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3497 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/bert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6957 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3561 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2619 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2852 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/bert/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      681 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/camembert/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3579 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/falcon/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2803 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/falcon/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6335 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/falcon/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3420 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/falcon/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3874 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/falcon/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (122)      157 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2834 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6950 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3997 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/gpt_neox/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4460 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (122)      140 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/llama/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2823 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/llama/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6528 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/llama/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/llama/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3893 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/llama/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4482 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/module.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4764 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3302 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2155 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2684 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       33 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      682 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/models/xlm_roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.017990 curated-transformers-0.9.0/curated_transformers/quantization/
--rw-r--r--   0 vsts      (1001) docker     (122)      126 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/quantization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/quantization/bnb/
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/quantization/bnb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2505 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/quantization/bnb/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5982 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/quantization/bnb/impl.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1101 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/quantization/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)      677 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/quantization/quantizable.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3002 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/generation/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      847 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/test_auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4647 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/test_dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4514 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4539 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/test_generic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2522 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/test_logits.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2860 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/generation/test_stop.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      703 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/albert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/bert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/camembert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2550 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/falcon/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.021990 curated-transformers-0.9.0/curated_transformers/tests/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1378 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3916 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/gpt_neox/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1367 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/llama/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3917 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/llama/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      511 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/roberta/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3789 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/test_attention.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2008 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/test_auto_models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3415 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/test_embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1324 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/models/xlm_roberta/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/quantization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/quantization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3732 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/quantization/test_generation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10744 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10642 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      733 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10778 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      977 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/test_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3909 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.025990 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/toy-roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30593 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
--rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/tokenizers/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.029990 curated-transformers-0.9.0/curated_transformers/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2924 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/_hf_compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3523 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2661 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3021 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.029990 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)      385 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2325 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/_fairseq.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11948 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4435 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7336 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2781 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4092 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2250 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3230 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3885 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11770 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      221 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.029990 curated-transformers-0.9.0/curated_transformers/util/
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/util/hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1208 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/util/pytorch.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7392 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/curated_transformers/util/serde.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 12:58:37.009990 curated-transformers-0.9.0/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     4313 2023-07-13 12:58:36.000000 curated-transformers-0.9.0/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     7667 2023-07-13 12:58:37.000000 curated-transformers-0.9.0/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 12:58:36.000000 curated-transformers-0.9.0/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       93 2023-07-13 12:58:36.000000 curated-transformers-0.9.0/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-07-13 12:58:36.000000 curated-transformers-0.9.0/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 12:58:36.000000 curated-transformers-0.9.0/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)      725 2023-07-13 12:58:37.029990 curated-transformers-0.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-07-13 12:58:26.000000 curated-transformers-0.9.0/setup.py
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

### Comparing `curated-transformers-0.9.0/LICENSE` & `curated-transformers-1.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/PKG-INFO` & `curated-transformers-1.0.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.9.0
-Summary: A PyTorch library of transformer models and components
+Version: 1.0.0.dev0
+Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `curated-transformers-0.9.0/README.md` & `curated-transformers-1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/_compat.py` & `curated-transformers-1.0.0.dev0/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/auto_generator.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/default_generator.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/default_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/dolly_v2.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/falcon.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/generator.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/generator_wrapper.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/generator_wrapper.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/hf_hub.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/logits.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/state.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/state.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/stop_conditions.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/generation/string_generator.py` & `curated-transformers-1.0.0.dev0/curated_transformers/generation/string_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/__init__.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/activations.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/attention.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/cache.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/cache.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/embeddings.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/feedforward.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/normalization.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/layers/scalar_weight.py` & `curated-transformers-1.0.0.dev0/curated_transformers/layers/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/albert/_hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/albert/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/albert/encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/albert/layer_group.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/auto_model.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/bert/_hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/bert/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/bert/embeddings.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/bert/encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/bert/layer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/camembert/encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/falcon/_hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/falcon/causal_lm.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/falcon/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/falcon/decoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/falcon/layer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/gpt_neox/_hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/gpt_neox/causal_lm.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/gpt_neox/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/gpt_neox/decoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/gpt_neox/layer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/hf_hub.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/llama/_hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/llama/causal_lm.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/llama/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/llama/decoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/llama/layer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/module.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/module.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/output.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/roberta/_hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/roberta/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/roberta/embeddings.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/roberta/encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/models/xlm_roberta/encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/quantization/bnb/config.py` & `curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/quantization/bnb/impl.py` & `curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/impl.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/quantization/helpers.py` & `curated-transformers-1.0.0.dev0/curated_transformers/quantization/helpers.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/quantization/quantizable.py` & `curated-transformers-1.0.0.dev0/curated_transformers/quantization/quantizable.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/conftest.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/generation/test_auto_generator.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/generation/test_dolly_v2.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/generation/test_falcon.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/generation/test_generic.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_generic.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/generation/test_logits.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/generation/test_stop.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_stop.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/albert/test_encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/camembert/test_encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/falcon/test_decoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/gpt_neox/test_decoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/llama/test_causal_lm.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/llama/test_decoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/test_attention.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/test_auto_models.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_auto_models.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/test_embeddings.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/test_hf_hub.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/util.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/models/xlm_roberta/test_encoder.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/quantization/test_generation.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/test_generation.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy.model` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/test_chunks.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/test_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tests/tokenizers/util.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/_hf_compat.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/_hf_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/auto_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/chunks.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/hf_hub.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/_fairseq.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/_fairseq.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/bert_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/llama_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/tokenizers/tokenizer.py` & `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/util/hf.py` & `curated-transformers-1.0.0.dev0/curated_transformers/util/hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/util/pytorch.py` & `curated-transformers-1.0.0.dev0/curated_transformers/util/pytorch.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers/util/serde.py` & `curated-transformers-1.0.0.dev0/curated_transformers/util/serde.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-1.0.0.dev0/curated_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.9.0
-Summary: A PyTorch library of transformer models and components
+Version: 1.0.0.dev0
+Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `curated-transformers-0.9.0/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-1.0.0.dev0/curated_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.9.0/setup.cfg` & `curated-transformers-1.0.0.dev0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-version = 0.9.0
-description = A PyTorch library of transformer models and components
+version = 1.0.0.dev0
+description = Curated transformer models
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
```

